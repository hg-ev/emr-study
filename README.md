# EMR Study

#### Tutorials
https://docs.aws.amazon.com/emr/latest/ManagementGuide/emr-gs.html

#### Quickstart
1. Generate a keypair with EC2
2. Setup S3 bucket with the python and csv files in this repo
3. Run ```aws emr create-cluster \
--name "My First EMR Cluster" \
--release-label emr-5.33.0 \
--applications Name=Spark \
--ec2-attributes KeyName=myEMRKeyPairName \
--instance-type m5.xlarge \
--instance-count 3 \
--use-default-roles```
