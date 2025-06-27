# CatFLW 😻
`Cat Facial Landmarks in the Wild (CatFLW)` dataset contains 2079 images of cats' faces in various environments and conditions, annotated with 48 facial landmarks and a bounding box on the cat’s face.

You can download the `CatFLW` dataset from [Kaggle](https://www.kaggle.com/datasets/georgemartvel/catflw).

Some examples from the dataset:
![](/good_cats.png)

## Scheme

The 48 cat facial landmarks were introduced in [Finka et al.](https://www.nature.com/articles/s41598-019-46330-5) and were specifically chosen for their relationship with underlying musculature and relevance to cat-specific facial Action Units ([CatFACS](https://animalfacs.com/catfacs_new)). You can find more details in the [dataset paper](https://arxiv.org/abs/2305.04232).

## Format

```
CatFLW/
│
├── images/
│ ├── 00000001_000.png
│ │ ...
│ └── CAT_01_00000184_024.png
└── labels/ 
  ├── 00000001_000.json
  │ ├── "labels" # (48,2)
  │ └── "bounding_boxes" # (x_1, y_1, x_2, y_2)
  │ ...
  └── CAT_01_00000184_024.json 
```

## References

If you use the `CatFLW`, please cite the [dataset paper](https://arxiv.org/abs/2305.04232):

```
@article{martvel2023catflw,
  title={Catflw: Cat facial landmarks in the wild dataset},
  author={Martvel, George and Farhat, Nareed and Shimshoni, Ilan and Zamansky, Anna},
  journal={arXiv preprint arXiv:2305.04232},
  year={2023}
}
```

You can also check out the [landmark detection paper](https://link.springer.com/article/10.1007/s11263-024-02006-w) and compare the detection performance on the CatFLW:

```
@article{martvel2024automated,
  title={Automated Detection of Cat Facial Landmarks},
  author={Martvel, George and Shimshoni, Ilan and Zamansky, Anna},
  journal={International Journal of Computer Vision},
  pages={1--16},
  year={2024},
  publisher={Springer}
}
```

## Contributions and Acknowledgements

The dataset was created by [Tech4Animals Lab](https://www.tech4animals.org) and supported by the [Data Science Research Center](https://dsrc.haifa.ac.il/?playlist=1d7a133&video=c6e22b5) at the University of Haifa. We thank Ephantus Kanyugi for his contribution to data annotation and management and Yaron Yossef for his technical support.

## License
This dataset is licensed under the Creative Commons Attribution-NonCommercial 4.0 International License.
https://creativecommons.org/licenses/by-nc/4.0/
