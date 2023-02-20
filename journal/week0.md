# Week 0 — Billing and Architecture

During week 0, I was given a project scenario by Margaret.

I was tasked with creating an ephemeral microblogging platform named Cruddr.

I learned about gathering requirements, and practiced making a conceptual diagram
 - both in napkin form, as well as in Lucid Chart!
 - 
![conceptual_napkin_diagram](https://user-images.githubusercontent.com/125823746/220016075-e858f4ca-40d1-45ce-823b-77e7e08d241f.jpg)


![lucid_chart_conceptual](https://user-images.githubusercontent.com/125823746/220016278-7d1a4d88-d453-4758-a86b-09e73cd4a107.png)

https://lucid.app/lucidchart/38f91f7f-1fbf-462f-9a79-95c049e92218/edit?viewport_loc=464%2C-272%2C2219%2C1047%2C0_0&invitationId=inv_c3b3a6fa-2c56-4bd1-a690-5b83e93ee8a4

Obstacles included difficulty trying to use Cloudshell - it would not load in my browser despite being in Northern Virginia region, and using a recent version of Firefox.

I ended up installing AWS CLI locally instead, and after running aws configure, was able to get a successful response to aws sts get-caller-identity.

Attempted homework challenges - made sure there wasn't inappropriate root account credentials, set up an IAM user, and set MFA.
