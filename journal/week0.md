# Week 0 — Billing and Architecture

I was given a project scenario by Margaret in the first Week 0 video, where I was tasked with creating an ephemeral microblogging platform named Cruddur.

## Required Homework / Tasks


### Recreate Conceptual Diagram in Lucid Charts or on a Napkin

I learned about gathering requirements, and practiced making a conceptual diagram both in napkin form, as well as in Lucidchart!

![napkin_diagram](https://user-images.githubusercontent.com/125823746/222904671-9bce686c-b79e-44b9-a3fe-4443abbeb452.png)




![lucid_chart_conceptual](https://user-images.githubusercontent.com/125823746/220016278-7d1a4d88-d453-4758-a86b-09e73cd4a107.png)

[Link](https://lucid.app/lucidchart/38f91f7f-1fbf-462f-9a79-95c049e92218/edit?viewport_loc=464%2C-272%2C2219%2C1047%2C0_0&invitationId=inv_c3b3a6fa-2c56-4bd1-a690-5b83e93ee8a4) to Lucid chart

### Recreate Logical Architectual Diagram in Lucid Charts

[Here](https://lucid.app/lucidchart/3d7e4afd-dd1a-49ff-ab74-9df3cb00c1a5/edit?invitationId=inv_31f663c5-0a9e-4aee-81a9-b6038880dbad) is the logical diagram I recreated in Lucidchart.

![logical_lucid_chart](https://user-images.githubusercontent.com/125823746/222957967-d92c5480-8e6d-4575-95a4-5cb1a1d71520.png)

Finding the icons I wanted was a bit time-consuming, though I'm getting better at navigating while making these charts.


### Create a Billing Alarm

I created a billing alarm to go off at $2.

![billing_alert](https://user-images.githubusercontent.com/125823746/222908193-3195f212-109d-46e9-afc7-a2f5e8fcfb13.png)



### Create a Budget

I created 2 budgets - 

- A zero spend budget, which would send a notification if anything was spent.
- A credit usage budget, which would send a notification if 75% of $4 ($3) in credits was used.


![my_budgets](https://user-images.githubusercontent.com/125823746/222908298-44189e0e-f459-46eb-99ba-561d4c039907.png)



## Obstacles

Obstacles included difficulty trying to use AWS CloudShell - it would not load in my browser despite double-checking that I was in Northern Virginia (a supported region) and using a recent version of Firefox (AWS documentation states the latest 3 versions should be supported.)

I ended up installing the AWS CLI locally instead, and after running aws configure, was able to get a successful response to aws sts get-caller-identity.

I used the installation instructions found [here](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html):

```
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
unzip awscliv2.zip
sudo ./aws/install
```

After configuring my setup with my credentials, I verified that it had my account information:




![aws_cli_local](https://user-images.githubusercontent.com/125823746/222904382-6c1ba8da-7de9-493e-b17d-dd1b8506c311.png)


and I was able to use the CLI successfully after that!


## Homework Challenges

### Made sure there weren't inappropriate root account credentials, set up an IAM user, and set MFA.

### Open a support ticket and request a service limit


![support_case](https://user-images.githubusercontent.com/125823746/222909521-284e7b89-3e84-41ec-b357-4611ded772d6.png)

I opened a ticket to increase the amount of CloudFront distributions... in doing so, I ended up resolving my earlier issue after speaking with support.
There was an additional verification that needed to be completed for my account, which after completing, allowed me to access AWS CloudShell!



