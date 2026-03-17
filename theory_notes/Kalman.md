# Kalman Filter
1. 简述：
   线性系统状态方程，通过输入输出（预测数据）观测数据对系统状态进行最优估计的算法。由于观测数据收到系统、环境的 **噪声和干扰** 影响，所以最优估计也可以看作滤波过程。（将不太准确的（预测、量测）融合为较为准确的估计的过程）
2. preliminary：
   1. **高斯（正太）分布**
      - <img width="725" height="189" alt="0af713d6af784fb0b916959f77b9fa5f" src="https://github.com/user-attachments/assets/88cd5f83-f26c-4228-bacd-34faf1e1b37d" />
   2. **协方差矩阵**： 方差、协方差在一个矩阵中表示出来
      - ![Uploading image.png…]()
> 符号说明：
   $\tilde$

$$
\hat{x}_k\,\,\text{最优估计值}\left( k\text{时刻} \right) 
\\
P_k\,\,\text{状态协方差}
\\
{\hat{x}_k}^-\,\,\text{状态预测值，}z_k\,\,\text{观测状态值}
\\
{P_k}^-\,\,\text{预测协方差矩阵，}R_k\,\,\text{观测方差，}Q_k\,\,\text{过程误差}
\\
H\,\,\text{映射矩阵}/\text{观测矩阵} K\text{卡尔曼增益}
\\
F\left( \varPhi \right) \,\,\text{状态转移矩阵}
$$
