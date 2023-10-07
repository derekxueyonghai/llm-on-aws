# llm-on-aws

large language models on AWS Youtube video tutorial. 

Following through each video. Git back the notebook run. 

Part 1: Introduction to foundation models

https://github.com/aws/amazon-sagemaker-examples/blob/main/introduction_to_amazon_algorithms/jumpstart-foundation-models/text-generation-falcon.ipynb 

Part 2: Picking the right foundation model

https://github.com/aws-samples/sagemaker-distributed-training-workshop/blob/main/10_llm_eval/Falcon40B_ROUGE.ipynb

Part 3:

https://github.com/aws/amazon-sagemaker-examples/blob/main/introduction_to_amazon_algorithms/jumpstart-foundation-models/domain-adaption-finetuning-gpt-j-6b.ipynb

Part 4: Pretraining a new foundation model

https://github.com/aws/amazon-sagemaker-examples/blob/main/training/distributed_training/pytorch/model_parallel/gpt2/smp-train-gpt-sharded-data-parallel.ipynb

'''
client = boto3.client("sts")
'''
'sts' security token service. This is useful for applications that need to access AWS resources but do not have their own long-term credentials.

https://www.youtube.com/watch?v=0xfe54_pYIQ

distribution --> 'mpi': message passing interface, 'ddp': distributed data parallel

Search for "parallel training in sagemaker" "parallel training in vertex at" 

Part 5: Preparing data and training at scale

https://github.com/aws/amazon-sagemaker-examples/blob/main/training/distributed_training/pytorch/model_parallel/gpt2/smp-train-gpt-sharded-data-parallel.ipynb

training by using fsx file system

use aws ecr container service

'humanize' library

Part 6: RL with human feedback

https://github.com/aws-samples/sagemaker-distributed-training-workshop/blob/main/9_rlhf/RLHF_locally.ipynb

ml.g4dn.xlarge	4	16 GiB	$0.7364


Part 7: Deploying a foundation model

https://github.com/aws/amazon-sagemaker-examples/blob/main/inference/nlp/realtime/llm/bloom_176b/djl_deepspeed_deploy.ipynb

ml.m5.large	2	8 GiB	$0.115
ml.t3.medium	2	4 GiB	$0.05

'''
image_uris.retrieve(
    framework="djl-deepspeed"
'''

hugging face sagemaker example notebook    

https://github.com/huggingface/notebooks/blob/main/sagemaker/27_deploy_large_language_models/sagemaker-notebook.ipynb

"Today is the hottest day "
