1.只用 Tensorflow 库，不需要 Keras 了；
2.每 1000 步会保存一次 weights，如果终止了程序，下次可以 load 进来，使用
	python3 categoricalDQN.py load 即可；
3.多个游戏分别写在 list: games 中，每个游戏运行最多 agent.episodes 次以及最多 Max_t 步；
4.每个游戏的结果保存在 result.txt 中:格式为： 名称,分数,总步数
5.参数 agent.timestep_per_train 用来调整多少步训练一次，感觉很重要