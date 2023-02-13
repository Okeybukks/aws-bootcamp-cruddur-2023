# Week 0 — Billing and Architecture

## Billing Alarm

For this task, I used AWS Cloudwatch to setup billing alert of 10 dollars. The cloudwatch sends spend warning of my monthly resource consumption to my email if the set 10 dollar mark is exceeded using AWS SNS.

![Alt text](/Week0_Documents/week0image1.png)

![Alt text](/Week0_Documents/week0image2.png)

## AWS Budget

To ensure one doesn't have a resource that keeps running and generating unintended cost, an AWS monthly budget of 10 dollars was created. It sends email notifications when the budget is about to be exceeded.

![Alt text](/Week0_Documents/week0image3.png)

## Logical Architectual Diagram of our Crudurr Application

The Logical Architectual Diagram of the Crudurr app I deseigned using Lucid can be found [here](https://lucid.app/lucidchart/a1f50200-0c75-4ab0-9b7f-911a318b7ae3/edit?viewport_loc=-410%2C-194%2C2601%2C1430%2C0_0&invitationId=inv_9cd4cca3-e6fd-4f98-ba8b-219bdfc17ddc "Lucid Diagram").

![Lucid Diagram](/Week0_Documents/week0image4.png)

## Conceptual Architectual Diagram of our Crudurr Application

The Conceptual Architectual Diagram of the Crudurr app I deseigned using Lucid can be found [here](https://lucid.app/lucidchart/a1f50200-0c75-4ab0-9b7f-911a318b7ae3/edit?viewport_loc=65%2C-119%2C1698%2C934%2CLeYw.~qmtn7t&invitationId=inv_9cd4cca3-e6fd-4f98-ba8b-219bdfc17ddc "Lucid Diagram").

![Lucid Diagram](/Week0_Documents/week0image5.png)