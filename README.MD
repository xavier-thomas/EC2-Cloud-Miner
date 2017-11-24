# EC2-Cloud-Miner
A Cloudformation template to mine cryptocurrency on AWS EC2


## Instructions for use.

1. Create an account on https://minergate.com/
2. Launch the cloudformation.yaml template on AWS Cloudformation
3. Configure the options based on what you want to do. Make sure you change the email address parameter to the email address you used to sign up to minergate.
4. Ensure you have a RSA keypair generated or uploaded to ec2.
5. Choose an instance type. (Through experimentation I have found that the M4 series works best. Due to the use of Intel Xeon E5-2686 v4 (Broadwell) processors) and the lower spot costs when compared to the other instances that use the same processor.
6. Choose a Coin to use. Monero (XMR) is currently the most profitable. Bytecoin (BCN) is the second most profitable.
7. Launch the template. Sit back and watch the cash roll in.


## Notes:

Mining on EC2 is not profitable. I created this template to use because I had some free credits from an AWS event and no other use for it.

I suggest using spot pricing to take advantage of the lower cost. You need to do your own research based on region to pick the best spot bid for your needs.

GPU mining does not currently work. The miner applications I was able to find only support AMD GPUs. All EC2 instances use NVDIA GPUs. I am attempting to find an alternative.
