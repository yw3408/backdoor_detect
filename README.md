# BBD:Bimodel Backdoor Defence

BBD is a Backdoor Defence Technique design for correctly recognize clean data and identify poisoned data as `N+1` Label.  To see the implementation, please open `src/BBD.ipythnb`,  and run file

## Group Member

Yuanrui Huang(yh2910)

Yihong Wang(yw3408)

Jiru Wang(jw6288)

Yichen Wang(yw4604)

## Evironment

`Python=>3.x`

`Jupyter Notebook`

`Tensorflow == 1.x`(for`neural_clease.ipythnb` to run)

`tensorflow-model-optimization`

`Keras => 2.x`

`h5py`

## HOWTO

 To run source code in `/src`, please open codefiles in Jupyter Notebook and modify data and model path into your own customized path.

`Fine_Pruning_Weight_Pruning.ipynb`

* `clean_data_filename` => customized clean validation data path
* `test_data_filename` =>customized clean test data path
* `poison_data_filename`=>customized poison data path

`Fine_Pruning_activation_based.ipynb`

* `clean_data_filename` => customized clean validation data path
* `test_data_filename` =>customized clean test data path
* `poison_data_filename`=>customized poison data path

`Entropy_filter.ipythnb`

* `clean_data_filename` =>customized clean validation data path

* `test_clean_data_filename` =>customized clean test  data path

* `poison_data_filename` => customized poison data path

  

`neural_clease.ipythnb`

* `DATA_DIR` => customized data folder

* `DATA_FILE` => customized clean data path

* `MODEL_DIR` => customized model folder

* `MODEL_FILE` => customized Badnet path

  

`BBD.ipythnb`

* `DATA_DIR` => customized data folder
* `CLEAN_DATA_FILE` => customized clean validation data path
* `POISON_DATA_FILE`=> customized poison data path
* `MODEL_DIR` => customized model folder
* `BAD_MODEL_FILE` => customized Badnet path
* `CLEAN_MODEL_FILE` => customized clean model path

All files can run idenpendently and with differnt purpose.



## File Describtion

| File                                | Input                      | Output              | Describtion |
| ----------------------------------- | -------------------------- | ------------------- | ----------- |
| `neural_clease.ipythnb`             | `<Badnet, Clean_Data>`     | `potential_trigger` |             |
| `Fine_Pruning_Weight_Pruning.ipynb` | `<Badnet, Clean_Data>`     | `Repaired_Model`    |             |
| `Fine_Pruning_activation_based.ipynb` | `<Badnet, Clean_Data>`     | `Repaired_Model`    |             |
| `Entropy_filter.ipythnb`            | `<Pruned Badnet, Clean_Data, Poison_Data>` | `Entropy Filter` |             |
| `BBD.ipythnb`                       | `<Badnet, Repaired Model>` | `Expected Classification` |             |

## Reference

- [1] [Bryant Chen, Wilka Carvalho, Nathalie Baracaldo, Heiko Ludwig, Benjamin Edwards, Taesung Lee, Ian Molloy, and Biplav Srivastava. 2018. Detecting backdoor attacks on deep neural networks by activation clustering.](https://arxiv.org/abs/1811.03728)
- [2] [Yansong Gao, Change Xu, Derui Wang, Shiping Chen, Damith C Ranasinghe, and
Surya Nepal. 2019. Strip: A defence against trojan attacks on deep neural networks.](https://arxiv.org/abs/1902.06531)
- [3] [Yiming Li, Baoyuan Wu, Yong Jiang, Zhifeng Li, and Shu-Tao Xia. 2020. Backdoor
Learning: A Survey.](https://arxiv.org/abs/2007.08745)
- [4] [ Kang Liu, Brendan Dolan-Gavitt, and Siddharth Garg. 2018. FinePruning: Defending Against Backdooring Attacks on Deep Neural Networks.](https://arxiv.org/abs/1805.12185)
- [5] [B. Wang, Y. Yao, S. Shan, H. Li, B. Viswanath, H. Zheng, and B. Y. Zhao. 2019.
Neural Cleanse: Identifying and Mitigating Backdoor Attacks in Neural Networks.](https://people.cs.uchicago.edu/~huiyingli/publication/backdoor-sp19.pdf)
- [6] [Jiale Zhang, Junjun Chen, Di Wu, Bing Chen, and Shui Yu. 2019. Poisoning attack in federated learning using generative adversarial nets.](https://ieeexplore.ieee.org/document/8887357)

