# Week 0 — Billing and Architecture

I was given a project scenario by Margaret in the first Week 0 video, where I was tasked with creating an ephemeral microblogging platform named Cruddr.

## Required Homework / Tasks


### Recreate Conceptual Diagram in Lucid Charts or on a Napkin

I learned about gathering requirements, and practiced making a conceptual diagram both in napkin form, as well as in Lucid Chart!

![napkin_diagram](https://user-images.githubusercontent.com/125823746/222904671-9bce686c-b79e-44b9-a3fe-4443abbeb452.png)




![lucid_chart_conceptual](https://user-images.githubusercontent.com/125823746/220016278-7d1a4d88-d453-4758-a86b-09e73cd4a107.png)

[Link](https://lucid.app/lucidchart/38f91f7f-1fbf-462f-9a79-95c049e92218/edit?viewport_loc=464%2C-272%2C2219%2C1047%2C0_0&invitationId=inv_c3b3a6fa-2c56-4bd1-a690-5b83e93ee8a4) to Lucid chart

### Create a Billing Alarm

I created a billing alarm to go off at $2.





### Create a Budget

I created 2 budgets - 

- A zero spend budget, which would send a notification if anything was spent.
- A credit usage budget, which would send a notification if 75% of $4 ($3) in credits was used.








## Obstacles

Obstacles included difficulty trying to use Cloudshell - it would not load in my browser despite being double-checking that I was in Northern Virginia (a supported region) and using a recent version of Firefox (AWS documentation states the latest 3 versions should be supported.)

I ended up installing the AWS CLI locally instead, and after running aws configure, was able to get a successful response to aws sts get-caller-identity.

I used the installation instructions found [here](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html):

```
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
unzip awscliv2.zip
sudo ./aws/install
```

After configuring my setup with my credentials, I verified that it had my account information:




![aws_cli_local](https://user-images.githubusercontent.com/125823746/222904382-6c1ba8da-7de9-493e-b17d-dd1b8506c311.png)


and I was able to use it successfully after that!

## Homework Challenges

Attempted homework challenges - made sure there wasn't inappropriate root account credentials, set up an IAM user, and set MFA.
