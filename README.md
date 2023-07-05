# Instructions 

This repository is associated with the paper SPHERICAL CAPS DO NOT ALWAYS MAXIMIZE NEUMANN EIGENVALUES ON THE SPHERE by DORIN BUCUR, RICHARD LAUGESEN, ELOI MARTINET and MICKAEL NAHON. It aims at provinding the meshes used in the paper alongside two codes written in FreeFem++ allowing to generate a mesh and compute it's associated eigenvalue. The names of the folders corresponds to the value of the aperture $\varepsilon$ of the small holes. The name of each mesh corresonds to the angle $\theta$ defined such that $|B(\theta)| = |\Om_\varepsilon(\theta)|$.

To vizualize a mesh, you can use medit :
```
medit 0.06283185307179587/2.2463963522993238.mesh
```

Using FreeFem++, you can generate you own mesh (which should appear under the name of PuncturedMesh.mesh in the root directory) :
```
FreeFem++ generate_mesh.edp
```

Finally, you can compute the first 10 eigenvalues of any mesh the following way :
```
FreeFem++ compute_eigenvalues.edp 0.06283185307179587/2.2463963522993238.mesh
```

That's it !

We hope that you find those little scripts useful. For more experiments like this one, you can visit [my website](https://eloimartinet.github.io/).