---
title: 'Tutorial: Azure Active Directory integration with CorpTax | Microsoft Docs'
description: Learn how to configure single sign-on between Azure Active Directory and CorpTax.
services: active-directory
documentationCenter: na
author: jeevansd
manager: daveba
ms.reviewer: barbkess

ms.assetid: fdad2893-41f4-4056-b6d2-ec3d050eb350
ms.service: active-directory
ms.workload: identity
ms.tgt_pltfrm: na
ms.devlang: na
ms.topic: tutorial
ms.date: 12/17/2018
ms.author: jeedes

ms.collection: M365-identity-device-management
---
# Tutorial: Azure Active Directory integration with CorpTax

In this tutorial, you learn how to integrate CorpTax with Azure Active Directory (Azure AD).
Integrating CorpTax with Azure AD provides you with the following benefits:

* You can control in Azure AD who has access to CorpTax.
* You can enable your users to be automatically signed-in to CorpTax (Single Sign-On) with their Azure AD accounts.
* You can manage your accounts in one central location - the Azure portal.

If you want to know more details about SaaS app integration with Azure AD, see [What is application access and single sign-on with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-appssoaccess-whatis).
If you don't have an Azure subscription, [create a free account](https://azure.microsoft.com/free/) before you begin.

## Prerequisites

To configure Azure AD integration with CorpTax, you need the following items:

* An Azure AD subscription. If you don't have an Azure AD environment, you can get one-month trial [here](https://azure.microsoft.com/pricing/free-trial/)
* CorpTax single sign-on enabled subscription

## Scenario description

In this tutorial, you configure and test Azure AD single sign-on in a test environment.

* CorpTax supports **SP** initiated SSO

## Adding CorpTax from the gallery

To configure the integration of CorpTax into Azure AD, you need to add CorpTax from the gallery to your list of managed SaaS apps.

**To add CorpTax from the gallery, perform the following steps:**

1. In the **[Azure portal](https://portal.azure.com)**, on the left navigation panel, click **Azure Active Directory** icon.

	![The Azure Active Directory button](common/select_azuread.png)

2. Navigate to **Enterprise Applications** and then select the **All Applications** option.

	![The Enterprise applications blade](common/enterprise_applications.png)

3. To add new application, click **New application** button on the top of dialog.

	![The New application button](common/add_new_app.png)

4. In the search box, type **CorpTax**, select **CorpTax** from result panel then click **Add** button to add the application.

	 ![CorpTax in the results list](common/search_new_app.png)

## Configure and test Azure AD single sign-on

In this section, you configure and test Azure AD single sign-on with CorpTax based on a test user called **Britta Simon**.
For single sign-on to work, a link relationship between an Azure AD user and the related user in CorpTax needs to be established.

To configure and test Azure AD single sign-on with CorpTax, you need to complete the following building blocks:

1. **[Configure Azure AD Single Sign-On](#configure-azure-ad-single-sign-on)** - to enable your users to use this feature.
2. **[Configure CorpTax Single Sign-On](#configure-corptax-single-sign-on)** - to configure the Single Sign-On settings on application side.
3. **[Create an Azure AD test user](#create-an-azure-ad-test-user)** - to test Azure AD single sign-on with Britta Simon.
4. **[Create CorpTax test user](#create-corptax-test-user)** - to have a counterpart of Britta Simon in CorpTax that is linked to the Azure AD representation of user.
5. **[Assign the Azure AD test user](#assign-the-azure-ad-test-user)** - to enable Britta Simon to use Azure AD single sign-on.
6. **[Test single sign-on](#test-single-sign-on)** - to verify whether the configuration works.

### Configure Azure AD single sign-on

In this section, you enable Azure AD single sign-on in the Azure portal.

To configure Azure AD single sign-on with CorpTax, perform the following steps:

1. In the [Azure portal](https://portal.azure.com/), on the **CorpTax** application integration page, select **Single sign-on**.

    ![Configure single sign-on link](common/select_sso.png)

2. On the **Select a Single sign-on method** dialog, select **SAML/WS-Fed** mode to enable single sign-on.

    ![Single sign-on select mode](common/select_saml_option.png)

3. On the **Set up Single Sign-On with SAML** page, click **Edit** icon to open **Basic SAML Configuration** dialog.

	![Edit Basic SAML Configuration](common/edit_urls.png)

4. On the **Basic SAML Configuration** section, perform the following steps:

    ![CorpTax Domain and URLs single sign-on information](common/sp_intiated.png)

    In the **Sign-on URL** text box, type a URL:
    `https://asp.corptax.com`

8. On the **Set up Single Sign-On with SAML** page, In the **SAML Signing Certificate** section, click **Download** to download **Federation Metadata XML** and save it on your computer.

	![The Certificate download link](common/metadataxml.png)

### Configure CorpTax Single Sign-On

To configure single sign-on on **CorpTax** side, you need to send the downloaded **Federation Metadata XML** to [CorpTax support team](mailto:bgraves@corptax.com). They set this setting to have the SAML SSO connection set properly on both sides.

### Create an Azure AD test user

The objective of this section is to create a test user in the Azure portal called Britta Simon.

1. In the Azure portal, in the left pane, select **Azure Active Directory**, select **Users**, and then select **All users**.

    ![The "Users and groups" and "All users" links](common/users.png)

2. Select **New user** at the top of the screen.

    ![New user Button](common/new_user.png)

3. In the User properties, perform the following steps.

    ![The User dialog box](common/user_properties.png)

    a. In the **Name** field, enter **BrittaSimon**.

    b. In the **User name** field, type **brittasimon@yourcompanydomain.extension**  
    For example, BrittaSimon@contoso.com

    c. Select **Show password** check box, and then write down the value that's displayed in the Password box.

    d. Click **Create**.

### Assign the Azure AD test user

In this section, you enable Britta Simon to use Azure single sign-on by granting access to CorpTax.

1. In the Azure portal, select **Enterprise Applications**, select **All applications**, then select **CorpTax**.

	![Enterprise applications blade](common/enterprise_applications.png)

2. In the applications list, type and select **CorpTax**.

	![The CorpTax link in the Applications list](common/all_applications.png)

3. In the menu on the left, select **Users and groups**.

    ![The "Users and groups" link](common/users_groups_blade.png)

4. Click the **Add user** button, then select **Users and groups** in the **Add Assignment** dialog.

    ![The Add Assignment pane](common/add_assign_user.png)

5. In the **Users and groups** dialog select **Britta Simon** in the Users list, then click the **Select** button at the bottom of the screen.

6. If you are expecting any role value in the SAML assertion then in the **Select Role** dialog select the appropriate role for the user from the list, then click the **Select** button at the bottom of the screen.

7. In the **Add Assignment** dialog, click the **Assign** button.

### Create CorpTax test user

In this section, you create a user called Britta Simon in CorpTax. Work with [CorpTax support team](mailto:bgraves@corptax.com) to add the users in the CorpTax platform. Users must be created and activated before you use single sign-on.

### Test single sign-on

In this section, you test your Azure AD single sign-on configuration using the Access Panel.
When you click the CorpTax tile in the Access Panel, you should be redirected to the below CorpTax page- 

![image](media/corptax-tutorial/corptaxlogin.png)

In **Environment** text box, type your appropriate environment, you should be automatically signed in to the CorpTax for which you set up SSO. For more information about the Access Panel, see [Introduction to the Access Panel](https://docs.microsoft.com/azure/active-directory/active-directory-saas-access-panel-introduction).

## Additional Resources

- [List of Tutorials on How to Integrate SaaS Apps with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-saas-tutorial-list)

- [What is application access and single sign-on with Azure Active Directory?](https://docs.microsoft.com/azure/active-directory/active-directory-appssoaccess-whatis)

- [What is conditional access in Azure Active Directory?](https://docs.microsoft.com/azure/active-directory/conditional-access/overview)
