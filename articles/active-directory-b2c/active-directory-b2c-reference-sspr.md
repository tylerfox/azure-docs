---
title: Self-service password reset in Azure Active Directory B2C | Microsoft Docs
description: Demonstrates how to set up self-service password reset for your customers in Azure Active Directory B2C
services: active-directory-b2c
author: davidmu1
manager: mtillman

ms.service: active-directory
ms.workload: identity
ms.topic: conceptual
ms.date: 04/17/2018
ms.author: davidmu
ms.component: B2C
---

# Set up self-service password reset for your customers
With the self-service password reset feature, your customers who have signed up for local accounts can reset their passwords on their own. This significantly reduces the burden on your support staff, especially if your application has millions of customers using it on a regular basis. Currently, using a verified email address is the only supported recovery method.

> [!NOTE]
> This article applies to self-service password reset used in the context of a sign-in policy. If you need fully customizable password reset policies invoked from your app, see [this article](active-directory-b2c-reference-policies.md#create-a-password-reset-policy).
> 
> 

By default, your directory doesn't have self-service password reset turned on. Use the following steps to turn it on:

1. Sign in to the [Azure portal](https://portal.azure.com/) as the Subscription Administrator. This is the same work or school account or the same Microsoft account that you used to create your directory.
2. Open **Azure Active Directory** (in the navigation bar on the left side).
4. Set **Self service password reset enabled**  to **All**. 
5. Click **Save** at the top of the page. You're done!

To test, use the "Run now" feature on any sign-in policy that has local accounts as an identity provider. On the local account sign-in page (where you enter an email address and password, or a username and password), click **Can't access your account?** to verify the customer experience.

> [!NOTE]
> The self-service password reset pages can be customized by using the [company branding feature](../active-directory/fundamentals/customize-branding.md).
> 
> 

