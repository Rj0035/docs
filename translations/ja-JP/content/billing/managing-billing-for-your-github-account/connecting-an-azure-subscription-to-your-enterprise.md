---
title: Azure サブスクリプションを Enterprise に接続する
intro: 'Microsoft Enterprise Agreement を使用して、{% data variables.product.prodname_actions %}、{% data variables.product.prodname_registry %}、{% data variables.product.prodname_codespaces %}の使用を有効化して支払うことができます。'
redirect_from:
  - /github/setting-up-and-managing-your-enterprise/managing-your-enterprise-account/connecting-an-azure-subscription-to-your-enterprise
  - /github/setting-up-and-managing-billing-and-payments-on-github/connecting-an-azure-subscription-to-your-enterprise
  - /github/setting-up-and-managing-your-enterprise/connecting-an-azure-subscription-to-your-enterprise
versions:
  ghec: '*'
shortTitle: Azureサブスクリプションの接続
---

## Azure サブスクリプションと {% data variables.product.product_name %}

{% data reusables.enterprise-accounts.billing-microsoft-ea-overview %} 詳しい情報については、「[{% data variables.product.prodname_actions %} の支払いについて](/billing/managing-billing-for-github-actions/about-billing-for-github-actions)」および「[{% data variables.product.prodname_registry %} の支払いについて](/billing/managing-billing-for-github-packages/about-billing-for-github-packages)」を参照してください。

{% note %}

**Note:** If your enterprise account is on a Microsoft Enterprise Agreement, connecting an Azure subscription is the only way to use {% data variables.product.prodname_actions %} and {% data variables.product.prodname_registry %} beyond the included amounts, or to use {% data variables.product.prodname_codespaces %} at all.

{% endnote %}

After you connect an Azure subscription, you can also manage your spending limits.

- "[Managing your spending limit for {% data variables.product.prodname_registry %}](/billing/managing-billing-for-github-packages/managing-your-spending-limit-for-github-packages)"
- "[Managing your spending limit for {% data variables.product.prodname_actions %}](/billing/managing-billing-for-github-actions/managing-your-spending-limit-for-github-actions)"
- "[Managing your spending limit for {% data variables.product.prodname_codespaces %}](/billing/managing-billing-for-github-codespaces/managing-spending-limits-for-codespaces)"

## Azure サブスクリプションを Enterprise アカウントに接続する

Azure サブスクリプションに接続するには、サブスクリプションに対するオーナーのアクセス許可が必要です。

{% data reusables.enterprise-accounts.access-enterprise %}
{% data reusables.enterprise-accounts.settings-tab %}
{% data reusables.enterprise-accounts.billing-tab %}
{% data reusables.enterprise-accounts.payment-information-tab %}
1. [Payment Information] で、[**Add Azure Subscription**] をクリックします。
1. 画面の指示に従って Microsoft アカウントにサインインします。
1. [Permissions requested] という画面表示を確認します。 規約に同意する場合は、[**Accept**] をクリックします。
1. [Select a subscription] で、Enterprise に接続する Azure サブスクリプション ID を選択します。

   {% note %}

   **ノート:** {% data variables.product.company_short %}のサブスクリプション権限検証は、利用可能なサブスクリプションのリストを表示するために読み取りのみのアクセスを要求します。 Azureサブスクリプションを選択するには、サブスクリプションに対するオーナー権限を持っていなければなりません。 デフォルトのテナントが適切な権限を持っていない場合は、異なるテナントIDを指定しなければならないことがあります。 詳しい情報についてはMicrosoftのドキュメンテーションの[Microsoft ID プラットフォームと OAuth 2.0 認証コード フロー](https://docs.microsoft.com/en-us/azure/active-directory/develop/v2-oauth2-auth-code-flow#request-an-authorization-code)を参照してください。

   {% endnote %}
1. [**Connect**] をクリックします。

## Enterprise アカウントから Azure サブスクリプションを切断する

Azure サブスクリプションを Enterprise アカウントから切断すると、プランに含まれている金額以上の使用量を利用できなくなります。

{% data reusables.enterprise-accounts.access-enterprise %}
{% data reusables.enterprise-accounts.settings-tab %}
{% data reusables.enterprise-accounts.billing-tab %}
{% data reusables.enterprise-accounts.payment-information-tab %}
1. [Azure subscription] の下で、切断するサブスクリプション ID の右側にある [**{% octicon "trash" aria-label="The trash icon" %}**] をクリックします。
1. 画面表示を確かめてから、[**Remove**] をクリックします。
