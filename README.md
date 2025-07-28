# aws-nuke-explore
Explore aws-nuke features and it's capabilities
Pre: check

1. we need to run "aws-nuke" from EC2 instance or jumpbox.
2. make sure you have nuke-config.yaml and aws-nuke exe.
3. update "aws-nuke" with account you want to nuke and region should be in "us-west-1" region (means which region you want to delete resources.)
4. copy the aws admin credentials to /home/ssm-user/.aws/credentials
5. Run aws-nuke run --config nuke-config.yaml --no-alias-check and save the output with <account_num>dry_run.txt
6. Run aws-nuke run --config nuke-config.yaml --no-alias-check --no-dry-run
   and save the output with <account_num>nuke.txt
