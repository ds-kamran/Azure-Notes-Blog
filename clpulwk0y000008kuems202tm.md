---
title: "Day 02: Introduction to AZURE AD"
datePublished: Thu Dec 07 2023 02:56:20 GMT+0000 (Coordinated Universal Time)
cuid: clpulwk0y000008kuems202tm
slug: day-02-introduction-to-azure-ad
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1701917745351/408494f2-47be-47ca-b235-51b8b2733e6f.webp
ogImage: https://cdn.hashnode.com/res/hashnode/image/upload/v1701917776826/602fc32e-6a29-4fa4-9643-a469dfd0ee1c.png
tags: azure, azure-active-directory, activedirectory

---

Azure Active Directory : It is Microsoft's cloud-based identity and access management service, which help users to sign in and access resources.

We can use Azure AD to implement SSO.

Types of AD:

1) Free

2) Office 365 Apps

3) Premium 1

4) Premium 2

Cannot create a custom access unless you have premium 1 and premium 2.

**Azure AD Use Cases:**

Azure AD can authorize and authenticate to multiple source.

**Active directory vs Azure Active directory:**

**Active directory terminology:**

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1701903292026/8a6de447-35fb-4805-bb89-d86ce66cdbbb.png align="center")

**Tenant:** A tenant represented as an organization in Azure Active Directory.

\--&gt;A tenant is automatically created when we signup for Microsoft Azure,Microsoft Intune or Microsoft 365.

\--&gt;Each tenant is distinct and separate from other azure ad tenants.

**Domain services:** When moving from on-prem to cloud, AD does not support some domain service. Hence, Azure AD DS provides managed domain service.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1701903833009/644e68ac-9543-4909-a291-2074bbcfb9a4.png align="center")

**AD Connect:** is a hybrid service to connect your on-premise Active Directory to your Azure Account.

Features of AD Connect:

a) password has sync:

b) pass-throug authen:

c) federation integration:

d) synchronization:

e) health monitoring: AD connect health

**AD - User:** It represent an identity for a person or employee in our domain.

User: A user is generated inside a tenant to access azure resource

Guest user: A guest user is an user invited to access the limited resouce of Azure

AD Groups:

AD Assign access rights:

Direct assign

group assign

rule-base assignment

external authority assignment

External AD : it allows users from outside of the org to access our apps and resources.

**LAB 01:**

**Creating a Tenant**

Tenant is actually logical division of the users in an organization.

Microsoft Entra Id is new name for active directory.

  
One cannot create a B2B in Free tier.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1701906302359/b4f79388-3c84-4cba-958b-3672f451cd65.png align="center")

Go to configuration

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1701906321432/04e31ef9-f61f-4311-a392-b8185aef6ec1.png align="center")

Missed the option of Choosing the user type: Hence B2C is paid and B2B comes with P1, P2 package.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1701906355991/2cc3f5ee-ed60-4c88-abd0-0f12403632e7.png align="center")

**User and group:**

Ideally, before you create a user, you need to create a group. There is no hard and fast rule, but during user creation the option is there to choose one group.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1701906772297/12ee31e1-8b2e-4b92-b7bc-770570bd8ff9.png align="center")

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1701906905422/5d7420a9-f0d8-40a5-82fb-11f8dbe6bf41.png align="center")

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1701906933465/470c8428-5c5c-4342-8fad-8fb489e89b24.png align="center")

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1701907020951/f26925a1-bffb-4508-987f-43981ceb5363.png align="center")

deleted user remains in the deleted user list for 30 days before it gets deleted from the tenant, which could restored within 30 days of deletion.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1701907170408/8c1a4e3b-ae26-4033-ac96-447378fa859d.png align="center")

It also has dynamic groups features for P1 and P2.

**Guest user :**

make us invite user from another tenant.

In order to create a guest user one must invite the user using the email id using create user.

**Mass Import:**

We can mass import users uploading the CSV template. So to create bulk users at once.

**MFA:** disabled for free version.

Only available for P1 and P2.

Can create MFA for users for secure login.

Could be done for bulk user, in bulk update.

**Self-service password:**

User can reset password by themself going to the password reset section.

Can be used using P1 and P2.

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1701911597666/4060e40f-dc6e-40d9-a22c-6efab6af2de1.png align="center")

AZURE AD Cheat Sheet:

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1701911843231/0f44352f-55e6-46b9-a1cd-f40db8684102.png align="center")

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1701911887225/5ebb1740-c388-4097-97ab-55818489e5be.png align="center")

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1701911924101/7f3e56d8-7a02-436f-aaa4-2728a78fe4e9.png align="center")