Particle System Simulation
An interactive particle simulation in C++ with SFML, driven by a custom-built linear algebra engine. Click anywhere to spawn bursts of particles with realistic physics and smooth animations.

Built with: C++, SFML

Controls:

Left click — spawn 5 particles at cursor position
Escape — exit

How it works: Each particle is represented as a matrix of 2D vertex coordinates. Movement, rotation, and shrinking are applied each frame using custom-implemented matrix transformations — rotation matrices, scaling matrices, and translation matrices — rather than any external math library. Particles arc upward with randomized velocity, are pulled down by simulated gravity, spin at random speeds, and fade out over a time-to-live countdown.

Key concepts: Matrix multiplication, 2D linear transformations, Cartesian coordinate mapping, game loop architecture, SFML VertexArray rendering

Dependencies: SFML 2.x

Build: g++ main.cpp Engine.cpp Particle.cpp Matrices.cpp -o particles -lsfml-graphics -lsfml-window -lsfml-system
