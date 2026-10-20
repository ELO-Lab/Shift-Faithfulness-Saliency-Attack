# Sparse-Attack-To-Saliency-Map

### Quick Start

Run the ResNet18 batch configuration used by `script_sh/resnet18.sh`:

```sh
python run_batch.py \
	--model-name resnet18 \
	--num_sample 100 \
	--operator-strategy uniform \
	--eps 50 \
	--w-margin 0.0 \
	--w-del 0.5 \
	--w-ins 0.5 \
	--seed 22520691 \
	--fitness-function margin_loss_causal_faithfull \
	--output-root rivf_official/server_run_seed/GA/22520691/ \
	--explain-method simple_gradient
```

## Citation
If you find our work useful, please cite:
```bibtex
@inproceedings{khoatn-mmm2027,
  title={Few Pixels, Fragile Faithfulness: Evaluating Visual Explanations under Sparse Perturbations},
  author={Khoa Tran, Viet-Hang Duong, Ngoc Hoang Luong},
  booktitle={International Conference on Multimedia Modeling (MM)},
  year={2025}
}
```