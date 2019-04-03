# Visualizing Loss Landscape of Neural Nets: Adversarial Training

Refer to (loss-landscape)[https://github.com/tomgoldstein/loss-landscape] library. 

Example 2d visualization:

```mpirun -n 1 python plot_surface.py --mpi --cuda --model resnet32 --x=-1:1:51 --y=-1:1:51 --model_file my_models/resnet32_clean.resnet32.000100.pt --dir_type weights --xnorm filter --xignore biasbn --ynorm filter --yignore biasbn --plot```

and then:

```python plot_2D.py --surf_file <path_to_surf_file>```