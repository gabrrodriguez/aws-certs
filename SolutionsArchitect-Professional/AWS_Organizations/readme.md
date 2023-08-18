# AWS Organizations 

## Reference Architecture

## Vocabulary 
_root account_
> This is the parent node under which each of the other accounts will fall within a hierarchy. The root is a single node and it will establish the designated account as the _management account_.

_organizational units_
> When a parent / child hiearchy is established within the Organizations construct, the _children_ accounts will be known as `Organizational Units (OU)`. 

_policies_
> Within the `AWS Organizations` service there will be various _policies_ that can be invoked on the _Organizational Units_. For example there are 1. Service Control Policies (SCPs) 2. Tag Policies 3. AI services opt-out policies & 4. Backup policies.  

## Excercise - Create an AWS Organization

1. Go to AWS Console, and select `AWS Organizations`
> NOTE: AWS Organizations is a Global Service.
2. Click `Create Organizations` and you will be redirected to the following screen. 
> NOTE: This is where the `root` account is established. 
<p>
<img width="350" alt="image" src="https://github.com/gabrrodriguez/aws-certs/assets/126508932/a0e8048f-a061-4b6d-83a4-9fa8fa426f07">
</p>
3. Once the root (aka management account) is created click on `Policies` > `Service Control Policies` > `Enable Service Control Policies`
> NOTE: When you do this you will provide `FullAWSAccess` by default and this policy only applies to the `root` account. You cannot restrict any action on the `root` account. 
<p>
<img width="350" alt="image" src="https://github.com/gabrrodriguez/aws-certs/assets/126508932/d4fd464c-42f9-4686-8fd8-d6a1eb20b287">
</p>
4. On the console click `AWS Accounts` > `Add an AWS Account` > `Create an AWS account`. 