
### 测试原版代码能否运行
python generate_data.py --problem vrp --name validation --seed 4321
python generate_data.py --problem vrp --name test --seed 1234

CUDA_VISIBLE_DEVICES=2 python run.py --graph_size 20 --problem cvrp --baseline rollout --run_name 'vrp20_rollout' --val_dataset data/vrp/vrp20_validation_seed4321.pkl