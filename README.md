# NesTPP
A novel framework for learning latent information diffusion mechanism in online discussion forums.

This is a implementation of the nested self-exciting point process, as described in our paper:  
Chen Ling, Guangmo Tong, and Mozi Chen, [NesTPP: Modeling Thread Dynamics in Online Discussion Forums](https://arxiv.org/abs/2003.06051) (HT 2020)

## Requirements
This code is written in Python. To use it you will need:
- Numpy > 1.16
- Scipy > 1.2
- pandas

## Model
<a href="https://www.codecogs.com/eqnedit.php?latex=\dpi{120}&space;\large&space;\lambda_{main}(t)&space;=&space;\mu_{main}&space;&plus;&space;\sum_{i=1}^{m}\underbrace{\lambda_{reply}^{i}(t)&space;\cdot&space;p_i^{\gamma}\cdot&space;(t-t_i&space;&plus;&space;c)^{-(\eta&space;&plus;1)}}_{\psi_{main}(t)}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\dpi{120}&space;\large&space;\lambda_{main}(t)&space;=&space;\mu_{main}&space;&plus;&space;\sum_{i=1}^{m}\underbrace{\lambda_{reply}^{i}(t)&space;\cdot&space;p_i^{\gamma}\cdot&space;(t-t_i&space;&plus;&space;c)^{-(\eta&space;&plus;1)}}_{\psi_{main}(t)}" title="\large \lambda_{main}(t) = \mu_{main} + \sum_{i=1}^{m}\underbrace{\lambda_{reply}^{i}(t) \cdot p_i^{\gamma}\cdot (t-t_i + c)^{-(\eta +1)}}_{\psi_{main}(t)}" /></a>

## Usage
### Run the demo
```
python ntpp.py
```

### Data
The data can be access with this [link](https://drive.google.com/drive/folders/1uZudmS2y9npqG0sbfLy6AlduwFG32Kbg?usp=sharing). Please put the data folder in the folder of NesTPP to correctly read it.

## Cite
```
@article{ling2020nestpp,
  title={NesTPP: Modeling Thread Dynamics in Online Discussion Forums},
  author={Ling, Chen and Tong, Guangmo and Chen, Mozi},
  journal={arXiv preprint arXiv:2003.06051},
  year={2020}
}
```
