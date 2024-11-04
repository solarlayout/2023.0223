[![INFORMS Journal on Computing Logo](https://INFORMSJoC.github.io/logos/INFORMS_Journal_on_Computing_Header.jpg)](https://pubsonline.informs.org/journal/ijoc)

# Layout Optimization for a Large-Scale Grid-Connected Solar Power Plant

This archive is distributed in association with the [INFORMS Journal on
Computing](https://pubsonline.informs.org/journal/ijoc) under the [MIT License](LICENSE).

The software and data in this repository are a snapshot of data and results
that were used in the research reported on in the paper
[Layout Optimization for a Large-Scale Grid-Connected Solar Power Plant](https://doi.org/10.1287/ijoc.2023.0223) by Chong Wang, Qinghua Wu, Kai Pan, and Zuo-Jun Max Shen.

## Cite

To cite the contents of this repository, please cite both the paper and this repo, using their respective DOIs.

https://doi.org/10.1287/ijoc.2023.0223

https://doi.org/10.1287/ijoc.2023.0223.cd

Below is the BibTex for citing this snapshot of the repository.

```
@misc{Wang2024,
  author =        {Wang, Chong AND Wu, Qinghua AND Pan, Kai AND Shen, Zuo-Jun Max},
  publisher =     {INFORMS Journal on Computing},
  title =         {Dataset for layout optimization for a large-Scale grid-Connected solar power plant},
  year =          {2024},
  doi =           {10.1287/ijoc.2023.0223.cd},
  url =           {https://github.com/INFORMSJoC/2023.0223},
  note =          {Available for download at \url{https://github.com/INFORMSJoC/2023.0223}},
}
```

## Description

The goal of this repository is to share data and results related to the Integrated Location and Routing (ILR) problem within a large-scale solar power plant, solved using our exact solution approach.

## Data

The instances are originally collected from the Hubei Branch of the [State Grid Corporation of China](http://www.sgcc.com.cn/html/sgcc_main_en/index.shtml). All sensitive or confidential information has been appropriately desensitized.

Each instance (denoted by "district_`<span>`$a$-`<span>`$b$") represents a grid-connected solar power plant with a set of photovoltaic arrays (PVAs) continuously placed in a PV farm. Here, $a$ is the number of districts, and $b$ is an index representing different layout shapes. Each district in these plants has 109 slots of PVAs, one of which is removed to install an inverter.

Please see [data](data) directory to view the data and detailed descriptions.

## Results

The instances are originally collected from the Hubei Branch of the [State Grid Corporation of China](http://www.sgcc.com.cn/html/sgcc_main_en/index.shtml). All sensitive or confidential information has been appropriately desensitized.

Please see [results](results) directory to view the optimal solutions and detailed descriptions.

## Replicating

To replicate the results in [Figure 1](results/mult-test), do either

```
make mult-test
```

or

```
python test.py mult
```

To replicate the results in [Figure 2](results/sum-test), do either

```
make sum-test
```

or

```
python test.py sum
```

## Ongoing Development

This code is being developed on an on-going basis at the author's
[Github site](https://github.com/tkralphs/JoCTemplate).

## Support

For support in using this software, submit an
[issue](https://github.com/tkralphs/JoCTemplate/issues/new).
