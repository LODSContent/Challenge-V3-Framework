<!-- This will be used in labs on the page before Summary page that require an Azure trial subscription as well as a M365 trial subscription

Variable: ShowSubCancel 

Activity/Question: 
Replacement Token Alias: Question1
Text: ###To proceed, please review and check the box to confirm your understanding and agreement with the following terms:
Format: Multiple Choice,single answer
Answer: I understand that a Microsoft trial subscription is necessary to complete all related labs within this Challenge Series. The trial subscription is valid for 30 days from the date of creation.  I acknowledge that I must proactively cancel my Microsoft trial subscription, preferably no later than 25 days after the account creation date, to avoid being charged a subscription fee.
Blocks page navigation until answered: Enabled 
Show Results in Report: Enabled 

-->

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

#Cancel your subscription 
####Cancel your Azure subscription to avoid charges to your credit card.

>[+alert] Expand for guidance on canceling your Azure trial subscription.
- Open **Microsoft Edge**, go to +++https://portal.azure.com+++, sign in to the Microsoft Defender portal as +++@lab.Variable(GlobalAdmin)+++ using +++@lab.Variable(UserPassword)+++ as the password, and then dismiss all prompts.
- In the Azure portal, navigate to +++Cost Management and Billing+++.
- Select **Cost Management**.
- Expand **Billing** ant then select **Azure subscriptions**.
- Select the subscription that you want to cancel.
- At the top of page, select **Cancel subscription**.
- Choose **Just learning about the platform** as the Reason for cancellation and then select **Cancel subscription**.

>[!Note] After the subscription is canceled, a notification shows that the cancellation is complete.

>[!help] Want to learn more? Review the documentation on [how to cancel you Azure subscription](https://learn.microsoft.com/en-us/azure/cost-management-billing/manage/cancel-azure-subscription "Cancel your Azure Subscription").

####Turn off recurring billing in the Microsoft 365 admin center of your Microsoft 365 E5 (no Teams) trial subscription to avoid charges to your credit card. 

>[+alert] Expand for guidance on turning off recurring billing your Microsoft 365 E5 (no Teams) trial subscription.
- Open **Microsoft Edge**, go to +++https://admin.microsoft.com+++, sign in to the Microsoft Defender portal as +++@lab.Variable(GlobalAdmin)+++ using +++@lab.Variable(UserPassword)+++ as the password, and then dismiss all prompts.
- Expand **Billing** and then select **Licenses**.
- Select the **Microsoft 365 E5 (No Teams)** license.
- Select **Manage subscription details**.
- Select **Edit recurring billing**.
- Choose **Off** and then select **Save**.

>[!Note] When you turn off recurring billing for a subscription, it isn’t canceled. The subscription remains active until it expires. You can view the expiration date on the Your products page in the admin center.

>[!help] Want to learn more? Review the documentation on [how to turn off recurring billing in the Microsoft 365 admin center](https://learn.microsoft.com/en-us/microsoft-365/commerce/subscriptions/renew-your-subscription?view=o365-worldwide "Turn off recurring billing in the Microsoft 365 admin center").


####Wait 3 to 4 days and then remove your credit card from the Azure account.

>[+alert] Expand for guidance on removing your credit card from the account.
>
>**Note:** After 3 to 4 days, you will be able to remove the credit card associated with the cancelled subscription. Copy the following steps to a local document and complete them at a later time: 
>
>```-nocolor
>- Open Microsoft Edge, go to https://portal.azure.com, sign in to the Microsoft Defender portal as @lab.Variable(GlobalAdmin) using @lab.Variable(UserPassword) as the password, and then dismiss all prompts.
>- In the Azure portal, navigate to Cost Management and Billing.
>- Select Cost Management.
>- Expand Billing ant then select Payment methods.
>- Under Your credit and debit cards, next to the credit card you used for the trial subscription, select the triple dots icon (...) and then choose Delete.
>- Select Delete.
>```

:::

<br>

---

#Acknowledgement 

@lab.Activity(Question1)
