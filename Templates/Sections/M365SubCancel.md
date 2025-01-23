<!-- This will be used in labs on the page before Summary page that require an M365 trial subscription

Variable: ShowSubCancel 

Activity/Question: 
Replacement Token Alias: Question1
Text: ###To proceed, please review and check the box to confirm your understanding and agreement with the following terms:
Format: Multiple Choice,single answer
Answer: I understand that a Microsoft trial subscription is necessary to complete all related labs within this Challenge Series. The trial subscription is valid for 30 days from the date of creation.  I acknowledge that I must proactively cancel my Microsoft trial subscription, preferably no later than 25 days after the account creation date, to avoid being charged a subscription fee.
Blocks page navigation until answered: Enabled 
Show Results in Report: Enabled 

-->
<p>

#Before you end your lab 

- Do you plan to complete any of the related Challenge Labs below using your current trial subscription? 
*Select **Yes to proceed to acknowledgement** or select **No to proceed with cancelling your subscription**.*

    @lab.DropDownList(ShowSubCancel)[Yes,No]

    >!INSTRUCTIONS[](https://raw.githubusercontent.com/LODSContent/Challenge-V3-Framework/main/Templates/Sections/NextStepSeries/@lab.Variable(Series).md) 


>[!ALERT] **Reminder:**
>Your Microsoft trial subscription is needed to complete all related labs within this Challenge Series. Your trial subscription is valid for **30 days** from the date on which you created it. <br><br>
>**You must proactively cancel** your Microsoft trial subscription, preferably no later than 25 days after your account creation date, **or you will be charged a subscription fee**.

:::ShowSubCancel(ShowSubCancel=No)
<br>

---
####Turn off recurring billing in the Microsoft 365 admin center of your Microsoft 365 E5 (no Teams) and cancel your trial subscription to avoid charges to your credit card. 

>[+alert] Expand for guidance on turning off recurring billing your Microsoft 365 E5 (no Teams) trial subscription.
- Open **Microsoft Edge**, go to +++https://admin.microsoft.com+++, sign in to the Microsoft Defender portal as +++@lab.Variable(GlobalAdmin)+++ using +++@lab.Variable(UserPassword)+++ as the password, and then dismiss all prompts.
- Expand **Billing** and then select **Licenses**.
- Select the **Microsoft 365 E5 (No Teams)** license.
- Select **Manage subscription details**.
- Select **Edit recurring billing**.
- Choose **Off** and then select **Save**.
- Select **Cancel subscription**
- Select **Next**
- Choose **Our business needs have changed** and the select **Cancel now**
- Select **Done**

>[!Note] When you turn off recurring billing for a subscription, it isn’t canceled. The subscription remains active until it expires. You can view the expiration date on the Your products page in the admin center.

>[!help] Want to learn more? Review the documentation on [how to turn off recurring billing in the Microsoft 365 admin center](https://learn.microsoft.com/en-us/microsoft-365/commerce/subscriptions/renew-your-subscription?view=o365-worldwide "Turn off recurring billing in the Microsoft 365 admin center").

:::

<br>

---

</p>

#Acknowledgement 

@lab.Activity(Question1)
