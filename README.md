# Sinogram Inpainting
This project reconstructs sinograms with missing data (undersampled or limited angles).

For instance, the sinogram data (left) of the CT image (right) is shown below. </br></br>
![image](https://github.com/XDDz123/sinogram-inpainting/assets/20507222/2567b101-059e-4614-b99b-ea241972dae1)</br></br>
The "inpainting" process aims to fill in data missing from the scanning process, so that the CT image could still be reconstructed. </br></br>
![image](https://github.com/XDDz123/sinogram-inpainting/assets/20507222/8ac0a934-1665-4ce2-9932-4a7d9c4fd82b) </br></br>

## Mechanics
The inpainting process could be solved by the following:</br></br>
$\displaystyle \frac{\partial f}{\partial t} = -\alpha \mathcal{L}(f)f$ where $f \in \overline{\Omega}$ subject to $f = f^*$ over $\partial\Omega$</br></br>
Where $\overline{\Omega}$ is the missing region, $\Omega$ is the known data, and $\partial\Omega$ is the Dirichlet boundary.

## Sample Output
### Inpainted Sinograms
![image](https://github.com/XDDz123/sinogram-inpainting/assets/20507222/71e13037-f339-477d-b254-6e8535fc61cc)
### Reconstruction
![image](https://github.com/XDDz123/sinogram-inpainting/assets/20507222/a1e47c1f-fb97-4ed7-a031-6489859fd954)
