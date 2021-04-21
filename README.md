# federated-double-deep-Q_network-
A framework that exploits the potentials of distributed federated learning and double deep Q-networks to minimize joint energy and delay in IoT networks

# The overal process of federated learning is as follows:
1) train local models
2) upload models to aggregation unit (we use FedAvg for aggregation purpose)
3) models are aggregated together, and global model is obtained
4) all local models would be updated with the parameters of global model

# The overal process of reinforcement learning (DDQN) is as follows:
1) select a task from task queue
2) choose an offloading decision (action) whether randomly or by using online network
3) calculate the reward/cost of action by optimizing transmit power (in case of offloading) or local computation resource allocation (if local computation is selected)
   and feed it as cost funtion to the RL agent
4) if the task is processed before its acceptable deadline then the task is successfully processed and is removed from task queue, otherwise task is a failure and remains in the task queue to be processed under another action
5) the local training is done when task queue is empty


# Main Libraries used
Pandas,
Numpy,
Keras,
Scipy,
Matplotlib

