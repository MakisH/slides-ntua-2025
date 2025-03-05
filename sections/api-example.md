## Extra slide: Example of using the API

```python [1|5-11|12-16|17|24-25,29-30|32-37|43]
import precice, nutils

def main(young=4e6, density=3e3, poisson=0.3, nelems=2, solver_dt=0.01, npoints_per_elem=3):
    # Setup Nutils simulation... (mesh, equations, boundary conditions)

    # preCICE setup
    solver_process_index = 0
    solver_process_size = 1
    participant =
    precice.Participant("Solid", "../precice-config.xml",
                        solver_process_index, solver_process_size)
    vertex_ids = 
    participant.set_mesh_vertices(mesh_name, wall.eval(ns.X))

    participant.initialize()

    while participant.is_coupling_ongoing():
            if participant.requires_writing_checkpoint():
                checkpoint = timestep, arguments

            precice_dt = participant.get_max_time_step_size()
            dt = min(precice_dt, solver_dt)

            # read forces from participant at the end of the timestep
            force = participant.read_data("Solid-Mesh", "Force", vertex_ids, dt)

            timestep += 1

            arguments = dict(dt=dt, u0=arguments['u'], v0=arguments['v'], F=force)
            arguments = solver.solve_linear('u:testu,v:testv', res, arguments=arguments, constrain=cons)

            # write displacements to participant
            write_data = wall.eval(ns.u, **arguments)
            participant.write_data("Solid-Mesh", "Displacement", vertex_ids, write_data)

            # do the coupling
            participant.advance(dt)

            # read checkpoint if required
            if participant.requires_reading_checkpoint():
                timestep, arguments = checkpoint

    participant.finalize()
```