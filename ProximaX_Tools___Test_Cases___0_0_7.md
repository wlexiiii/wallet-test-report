::: {#page}
::: {#main .aui-page-panel}
::: {#main-header}
::: {#breadcrumb-section}
1.  [ProximaX Tools](index.html)
2.  [Test Reports](Test-Reports_2443871313.html)
:::

# [ ProximaX Tools : Test Cases - 0.0.7 ]{#title-text} {#title-heading .pagetitle}
:::

::: {#content .view}
::: page-metadata
Created by [ James Chew]{.author}, last modified by [ Khoo Kiat
Ling]{.editor} on Dec 29, 2021
:::

::: {#main-content .wiki-content .group}
Date: 6.9.2021 - 10.9.2021

Version: 0.0.7

Release Notes:

Test Environment: Edge (Version 93.0.961.38), Windows 10, Core i7-7700HQ
CPU, 8GB RAM, 1TB ROM

Staging Link: [ProximaX Web Wallet
(proximax-foundry.github.io)](https://proximax-foundry.github.io/web-wallet-vuejs/#/){.external-link
rel="nofollow"}

Browser: Microsoft Edge (Version 93.0.961.38)

Testnet: Testnet 1

Clickup Link:
[https://app.clickup.com/3632843/v/b/li/49534768](https://app.clickup.com/3632843/v/b/li/49534768){.external-link
card-appearance="inline" rel="nofollow"}

::: {.toc-macro .rbtoc1667369988751}
-   [Main Page](#TestCases-0.0.7-MainPage)
    -   [Sign In](#TestCases-0.0.7-SignIn)
    -   [Sign In With SiriusID](#TestCases-0.0.7-SignInWithSiriusID)
    -   [Create New Wallet](#TestCases-0.0.7-CreateNewWallet)
    -   [Create New Wallet From Private
        Key](#TestCases-0.0.7-CreateNewWalletFromPrivateKey)
    -   [Import wallet from .wlt
        file](#TestCases-0.0.7-Importwalletfrom.wltfile)
-   [Dashboard](#TestCases-0.0.7-Dashboard)
-   [Transfer](#TestCases-0.0.7-Transfer)
-   [Accounts](#TestCases-0.0.7-Accounts)
    -   -   [Create a New Account](#TestCases-0.0.7-CreateaNewAccount)

    -   [Select Creation Type](#TestCases-0.0.7-SelectCreationType)
        -   [Import Account](#TestCases-0.0.7-ImportAccount)

    -   [Edit an existing
        Account](#TestCases-0.0.7-EditanexistingAccount)
        -   [Details](#TestCases-0.0.7-Details)

    -   [Convert to Multisig](#TestCases-0.0.7-ConverttoMultisig)

    -   [Edit Multisig](#TestCases-0.0.7-EditMultisig)
-   [Services](#TestCases-0.0.7-Services)
    -   [Namespaces](#TestCases-0.0.7-Namespaces)
    -   [Assets](#TestCases-0.0.7-Assets)
    -   [Mainnet Swap](#TestCases-0.0.7-MainnetSwap)
    -   [Address Book](#TestCases-0.0.7-AddressBook)
    -   [Wallets](#TestCases-0.0.7-Wallets)
    -   [Nodes](#TestCases-0.0.7-Nodes)
    -   [Attestation](#TestCases-0.0.7-Attestation)
    -   [Notifications](#TestCases-0.0.7-Notifications)
    -   [Voting](#TestCases-0.0.7-Voting)
    -   [Storage](#TestCases-0.0.7-Storage)
    -   [Sirius Gift](#TestCases-0.0.7-SiriusGift)
    -   [Aggregate Transaction](#TestCases-0.0.7-AggregateTransaction)
        -   [Aggregate Complete](#TestCases-0.0.7-AggregateComplete)
:::

::: {.confluence-information-macro .confluence-information-macro-information}
[]{.aui-icon .aui-icon-small .aui-iconfont-info
.confluence-information-macro-icon}

::: confluence-information-macro-body
Status: [NOT READY]{.status-macro .aui-lozenge} [READY]{.status-macro
.aui-lozenge .aui-lozenge-current} [PASS]{.status-macro .aui-lozenge
.aui-lozenge-success} [FAIL]{.status-macro .aui-lozenge
.aui-lozenge-error}
:::
:::

::: table-wrap
+----------+----------+----------+----------+----------+----------+
| ## Main  |          |          |          |          |          |
| Page {#T |          |          |          |          |          |
| estCases |          |          |          |          |          |
| -0.0.7-M |          |          |          |          |          |
| ainPage} |          |          |          |          |          |
+----------+----------+----------+----------+----------+----------+
| **Test   | **Test   | **Test   | **       | **       | **       |
| Case     | Sce      | steps**  | Expected | Status** | Remark** |
| ID**     | narios** |          | result** |          |          |
+----------+----------+----------+----------+----------+----------+
| Main-1   | Sign in  | Click on | Go to    | [PAS     |          |
|          |          | "Sign    | screen   | S]{.stat |          |
|          |          | in"      | "Sign in | us-macro |          |
|          |          | button   | to your  | .aui     |          |
|          |          |          | wallet"  | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| Main-2   | Sign in  | Click on | Show the | [NOT     |          |
|          | with     | "Sign in | form     | READ     |          |
|          | SiriusID | with     | "Sign in | Y]{.stat |          |
|          |          | S        | your     | us-macro |          |
|          |          | iriusID" | wallet   | .aui-    |          |
|          |          | button   | by       | lozenge} |          |
|          |          |          | scanning |          |          |
|          |          |          | this QR  |          |          |
|          |          |          | Code     |          |          |
|          |          |          | using    |          |          |
|          |          |          | your     |          |          |
|          |          |          | SiriusID |          |          |
|          |          |          | app"     |          |          |
+----------+----------+----------+----------+----------+----------+
| Main-3   | Create   | Click on | Go to    | [PAS     |          |
|          |          | "Create" | screen   | S]{.stat |          |
|          |          | button   | "Select  | us-macro |          |
|          |          |          | Wallet   | .aui     |          |
|          |          |          | Creation | -lozenge |          |
|          |          |          | Type"    | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| ### S    |          |          |          |          |          |
| ign In { |          |          |          |          |          |
| #TestCas |          |          |          |          |          |
| es-0.0.7 |          |          |          |          |          |
| -SignIn} |          |          |          |          |          |
+----------+----------+----------+----------+----------+----------+
| SIGNIN-1 | Select a | Leave    | Show     | [PAS     |          |
|          | wallet   | the      | required | S]{.stat |          |
|          |          | field    | field    | us-macro |          |
|          |          | empty    | message  | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| SIGNIN-2 | Password | Leave    | Show     | [PAS     |          |
|          |          | the      | required | S]{.stat |          |
|          |          | field    | field    | us-macro |          |
|          |          | empty    | message  | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| SIGNIN-3 |          | Place    | Show     | [FAI     | No       |
|          |          | less     | message  | L]{.stat | message  |
|          |          | than     | of       | us-macro | is shown |
|          |          | required | minimum  | .aui     |          |
|          |          | values   | number   | -lozenge |          |
|          |          |          | of       | .au      |          |
|          |          |          | ch       | i-lozeng |          |
|          |          |          | aracters | e-error} |          |
|          |          |          | to enter |          |          |
+----------+----------+----------+----------+----------+----------+
| SIGNIN-4 |          | Enter    | Show an  | [PAS     |          |
|          |          | invalid  | error    | S]{.stat |          |
|          |          | password | message  | us-macro |          |
|          |          |          |          | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| SIGNIN-5 | N/A      | Click    | Enter    | [PAS     |          |
|          |          | on       | the      | S]{.stat |          |
|          |          | "Sign    | app      | us-macro |          |
|          |          | in"      | lication | .aui     |          |
|          |          | button   |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| SIGNIN-6 |          | Click on | Clear    | [PAS     |          |
|          |          | "Clear"  | the form | S]{.stat |          |
|          |          | button   |          | us-macro |          |
|          |          |          |          | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| SIGNIN-7 | General  | UI       | N/A      |          |          |
|          | form     | veri     |          |          |          |
|          |          | fication |          |          |          |
|          |          | (syntax) |          |          |          |
+----------+----------+----------+----------+----------+----------+
| ### Sig  |          |          |          | [NOT     |          |
| n In Wit |          |          |          | READ     |          |
| h Sirius |          |          |          | Y]{.stat |          |
| ID {#Tes |          |          |          | us-macro |          |
| tCases-0 |          |          |          | .aui-    |          |
| .0.7-Sig |          |          |          | lozenge} |          |
| nInWithS |          |          |          |          |          |
| iriusID} |          |          |          |          |          |
+----------+----------+----------+----------+----------+----------+
|          |          |          |          |          |          |
+----------+----------+----------+----------+----------+----------+
| ### Crea |          |          |          |          |          |
| te New W |          |          |          |          |          |
| allet {# |          |          |          |          |          |
| TestCase |          |          |          |          |          |
| s-0.0.7- |          |          |          |          |          |
| CreateNe |          |          |          |          |          |
| wWallet} |          |          |          |          |          |
+----------+----------+----------+----------+----------+----------+
| NEWWLT-1 | Create\  | Click on | Go to    | [PAS     |          |
|          | (New     | "        | screen   | S]{.stat |          |
|          | Wallet)  | Create - | "Create  | us-macro |          |
|          |          | New      | wallet " | .aui     |          |
|          |          | wallet"  |          | -lozenge |          |
|          |          | button   |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| NEWWLT-2 | Select   | Click on | Show the | [PAS     |          |
|          | network  | "Select  | a        | S]{.stat |          |
|          |          | network" | vailable | us-macro |          |
|          |          | button   | networks | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| NEWWLT-3 | Wallet   | Leave    | Show a   | [PAS     |          |
|          | name     | the      | message  | S]{.stat |          |
|          |          | field    |          | us-macro |          |
|          |          | empty    |          | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| NEWWLT-4 |          | Set      | N/A      | [PAS     |          |
|          |          | special  |          | S]{.stat |          |
|          |          | ch       |          | us-macro |          |
|          |          | aracters |          | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| NEWWLT-5 | P        | Leave    | Show a   | [PAS     |          |
|          | assword  | the      | message  | S]{.stat |          |
|          |          | field    |          | us-macro |          |
|          |          | empty    |          | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| NEWWLT-6 |          | Set an   | Show a   | [PAS     |          |
|          |          | invalid  | message  | S]{.stat |          |
|          |          | password |          | us-macro |          |
|          |          |          |          | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| NEWWLT-7 |          | Set      | N/A      | [PAS     |          |
|          |          | special  |          | S]{.stat |          |
|          |          | ch       |          | us-macro |          |
|          |          | aracters |          | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| NEWWLT-8 |          | Place    | Show     | [FAI     | No       |
|          |          | less     | message  | L]{.stat | message  |
|          |          | than     | of       | us-macro | is shown |
|          |          | required | minimum  | .aui     |          |
|          |          | values   | number   | -lozenge |          |
|          |          |          | of       | .au      |          |
|          |          |          | ch       | i-lozeng |          |
|          |          |          | aracters | e-error} |          |
|          |          |          | to enter |          |          |
+----------+----------+----------+----------+----------+----------+
| NEWWLT-9 | Confirm  | Leave    | Show a   | [PAS     |          |
|          | password | the      | message  | S]{.stat |          |
|          |          | field    |          | us-macro |          |
|          |          | empty    |          | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| N        |          | Set an   | Show a   | [PAS     |          |
| EWWLT-10 |          | invalid  | message  | S]{.stat |          |
|          |          | password |          | us-macro |          |
|          |          |          |          | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| N        |          | Set      | N/A      | [PAS     |          |
| EWWLT-11 |          | special  |          | S]{.stat |          |
|          |          | ch       |          | us-macro |          |
|          |          | aracters |          | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| N        |          | Place    | Show     | [FAI     | No       |
| EWWLT-12 |          | less     | message  | L]{.stat | message  |
|          |          | than     | of       | us-macro | is shown |
|          |          | required | minimum  | .aui     |          |
|          |          | values   | number   | -lozenge |          |
|          |          |          | of       | .au      |          |
|          |          |          | ch       | i-lozeng |          |
|          |          |          | aracters | e-error} |          |
|          |          |          | to enter |          |          |
+----------+----------+----------+----------+----------+----------+
| N        | Eye      | Click on | Show /   | [PAS     |          |
| EWWLT-13 | Icons    | "P       | hide the | S]{.stat |          |
|          |          | assword" | password | us-macro |          |
|          |          | eye icon |          | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| N        |          | Click on | Show /   | [PAS     |          |
| EWWLT-14 |          | "Confirm | hide the | S]{.stat |          |
|          |          | p        | password | us-macro |          |
|          |          | assword" |          | .aui     |          |
|          |          | eye icon |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| N        | Clear    | Click on | Clean    | [PAS     |          |
| EWWLT-15 |          | "Clear"  | the form | S]{.stat |          |
|          |          | button   |          | us-macro |          |
|          |          |          |          | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| N        | Create   | Click on | Send a   | [PAS     |          |
| EWWLT-16 |          | "Create" | conf     | S]{.stat |          |
|          |          | button   | irmation | us-macro |          |
|          |          |          | message  | .aui     |          |
|          |          |          | and      | -lozenge |          |
|          |          |          | create   | .aui-    |          |
|          |          |          | the      | lozenge- |          |
|          |          |          | wallet   | success} |          |
+----------+----------+----------+----------+----------+----------+
| ### Cre  |          |          |          |          |          |
| ate New  |          |          |          |          |          |
| Wallet F |          |          |          |          |          |
| rom Priv |          |          |          |          |          |
| ate Key  |          |          |          |          |          |
| {#TestCa |          |          |          |          |          |
| ses-0.0. |          |          |          |          |          |
| 7-Create |          |          |          |          |          |
| NewWalle |          |          |          |          |          |
| tFromPri |          |          |          |          |          |
| vateKey} |          |          |          |          |          |
+----------+----------+----------+----------+----------+----------+
| N        | Create\  | Click on | Go to    | [PAS     |          |
| EWWLT-17 | (From a  | "        | screen   | S]{.stat |          |
|          | Private  | Create - | "Create  | us-macro |          |
|          | Key)     | From a   | wallet   | .aui     |          |
|          |          | private  | from a   | -lozenge |          |
|          |          | key"     | private  | .aui-    |          |
|          |          | button   | key"     | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| N        | Select   | Click on | Show the | [PAS     |          |
| EWWLT-18 | network  | "Select  | a        | S]{.stat |          |
|          |          | network" | vailable | us-macro |          |
|          |          | button   | networks | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| N        | Private  | Leave    | Show an  | [PAS     |          |
| EWWLT-19 | key      | the      | error    | S]{.stat |          |
|          |          | field    | message  | us-macro |          |
|          |          | empty    |          | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| N        |          | Set an   | Show an  | [FAI     | No       |
| EWWLT-20 |          | invalid  | error    | L]{.stat | message  |
|          |          | value    | message  | us-macro | is shown |
|          |          |          |          | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .au      |          |
|          |          |          |          | i-lozeng |          |
|          |          |          |          | e-error} |          |
+----------+----------+----------+----------+----------+----------+
| N        | Swap     | Click on | Check    | [PAS     |          |
| EWWLT-21 |          | checkbox | the      | S]{.stat |          |
|          |          |          | option   | us-macro |          |
|          |          |          |          | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| N        | Wallet   | Leave    | Show a   | [PAS     |          |
| EWWLT-22 | name     | the      | message  | S]{.stat |          |
|          |          | field    |          | us-macro |          |
|          |          | empty    |          | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| N        |          | Set      | N/A      | [PAS     |          |
| EWWLT-23 |          | special  |          | S]{.stat |          |
|          |          | ch       |          | us-macro |          |
|          |          | aracters |          | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| N        | P        | Leave    | Show a   | [PAS     |          |
| EWWLT-24 | assword  | the      | message  | S]{.stat |          |
|          |          | field    |          | us-macro |          |
|          |          | empty    |          | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| N        |          | Set an   | Show a   | [FAI     | No       |
| EWWLT-25 |          | invalid  | message  | L]{.stat | message  |
|          |          | password |          | us-macro | is shown |
|          |          |          |          | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .au      |          |
|          |          |          |          | i-lozeng |          |
|          |          |          |          | e-error} |          |
+----------+----------+----------+----------+----------+----------+
| N        |          | Set      | N/A      | [PAS     |          |
| EWWLT-26 |          | special  |          | S]{.stat |          |
|          |          | ch       |          | us-macro |          |
|          |          | aracters |          | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| N        |          | Place    | Show     | [FAI     | No       |
| EWWLT-27 |          | less     | message  | L]{.stat | message  |
|          |          | than     | of       | us-macro | is shown |
|          |          | required | minimum  | .aui     |          |
|          |          | values   | number   | -lozenge |          |
|          |          |          | of       | .au      |          |
|          |          |          | ch       | i-lozeng |          |
|          |          |          | aracters | e-error} |          |
|          |          |          | to enter |          |          |
+----------+----------+----------+----------+----------+----------+
| N        | Confirm  | Leave    | Show a   | [PAS     |          |
| EWWLT-28 | password | the      | message  | S]{.stat |          |
|          |          | field    |          | us-macro |          |
|          |          | empty    |          | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| N        |          | Set an   | Show a   | [FAI     | No       |
| EWWLT-29 |          | invalid  | message  | L]{.stat | message  |
|          |          | password |          | us-macro | is shown |
|          |          |          |          | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .au      |          |
|          |          |          |          | i-lozeng |          |
|          |          |          |          | e-error} |          |
+----------+----------+----------+----------+----------+----------+
| N        |          | Set      | N/A      | [PAS     |          |
| EWWLT-30 |          | special  |          | S]{.stat |          |
|          |          | ch       |          | us-macro |          |
|          |          | aracters |          | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| N        |          | Place    | Show     | [FAI     | No       |
| EWWLT-31 |          | less     | message  | L]{.stat | message  |
|          |          | than     | of       | us-macro | is shown |
|          |          | required | minimum  | .aui     |          |
|          |          | values   | number   | -lozenge |          |
|          |          |          | of       | .au      |          |
|          |          |          | ch       | i-lozeng |          |
|          |          |          | aracters | e-error} |          |
|          |          |          | to enter |          |          |
+----------+----------+----------+----------+----------+----------+
| N        | Eye      | Click on | Show /   | [PAS     |          |
| EWWLT-32 | icons    | "Private | hide the | S]{.stat |          |
|          |          | key" eye | private  | us-macro |          |
|          |          | icon     | key      | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| N        |          | Click on | Show /   | [PAS     |          |
| EWWLT-33 |          | "P       | hide the | S]{.stat |          |
|          |          | assword" | password | us-macro |          |
|          |          | eye icon |          | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| N        |          | Click on | Show /   | [PAS     |          |
| EWWLT-34 |          | "Confirm | hide the | S]{.stat |          |
|          |          | p        | password | us-macro |          |
|          |          | assword" |          | .aui     |          |
|          |          | eye icon |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| N        | N/A      | Click on | Clean    | [PAS     |          |
| EWWLT-35 |          | "Clear"  | the form | S]{.stat |          |
|          |          | button   |          | us-macro |          |
|          |          |          |          | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| N        |          | Click on | Send a   | [PAS     |          |
| EWWLT-36 |          | "Create" | conf     | S]{.stat |          |
|          |          | button   | irmation | us-macro |          |
|          |          |          | message  | .aui     |          |
|          |          |          | and      | -lozenge |          |
|          |          |          | create   | .aui-    |          |
|          |          |          | the      | lozenge- |          |
|          |          |          | wallet   | success} |          |
+----------+----------+----------+----------+----------+----------+
| N        | General  | UI       | N/A      |          |          |
| EWWLT-37 | form     | veri     |          |          |          |
|          |          | fication |          |          |          |
|          |          | (syntax) |          |          |          |
+----------+----------+----------+----------+----------+----------+
| ###      |          |          |          |          |          |
| Import w |          |          |          |          |          |
| allet fr |          |          |          |          |          |
| om .wlt  |          |          |          |          |          |
| file {#T |          |          |          |          |          |
| estCases |          |          |          |          |          |
| -0.0.7-I |          |          |          |          |          |
| mportwal |          |          |          |          |          |
| letfrom. |          |          |          |          |          |
| wltfile} |          |          |          |          |          |
+----------+----------+----------+----------+----------+----------+
| NEWWLT-3 | Import\  | Click on | Open a   | [PAS     |          |
|          | (From a  | "        | browse   | S]{.stat |          |
|          | Wallet   | Import - | to       | us-macro |          |
|          | Backup)  | From a   | search   | .aui     |          |
|          |          | wallet   | the .wlt | -lozenge |          |
|          |          | backup"  | file     | .aui-    |          |
|          |          | button   |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
:::

::: table-wrap
+----------+----------+----------+----------+----------+----------+
| #        |          |          |          |          |          |
| # Dashbo |          |          |          |          |          |
| ard {#Te |          |          |          |          |          |
| stCases- |          |          |          |          |          |
| 0.0.7-Da |          |          |          |          |          |
| shboard} |          |          |          |          |          |
+----------+----------+----------+----------+----------+----------+
| **Test   | **Test   | **Test   | **       | **       | **R      |
| Case     | Sce      | steps**  | Expected | Status** | emarks** |
| ID**     | narios** |          | result** |          |          |
+----------+----------+----------+----------+----------+----------+
| DASH-1   | Transfer | Click on | Goes to  | [PAS     |          |
|          |          | "Tr      | "        | S]{.stat |          |
|          |          | ansfer". | Transfer | us-macro |          |
|          |          |          | \> Make  | .aui     |          |
|          |          |          | a        | -lozenge |          |
|          |          |          | tran     | .aui-    |          |
|          |          |          | saction" | lozenge- |          |
|          |          |          | page.    | success} |          |
+----------+----------+----------+----------+----------+----------+
| DASH-2   | Accounts | Click on | Goes to  | [PAS     |          |
|          |          | "A       | "        | S]{.stat |          |
|          |          | ccounts. | Accounts | us-macro |          |
|          |          |          | \>View   | .aui     |          |
|          |          |          | All"     | -lozenge |          |
|          |          |          | page.    | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| DASH-3   | Services | Click on | Shows    | [PAS     |          |
|          |          | "S       | all      | S]{.stat |          |
|          |          | ervices" | a        | us-macro |          |
|          |          |          | vailable | .aui     |          |
|          |          |          | s        | -lozenge |          |
|          |          |          | ervices. | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| DASH-4   | Change   | Click on | A list   | [PAS     |          |
|          | Account  | the      | of       | S]{.stat |          |
|          |          | account  | a        | us-macro |          |
|          |          | name     | vailable | .aui     |          |
|          |          | shown.   | accounts | -lozenge |          |
|          |          |          | will pop | .aui-    |          |
|          |          |          | up.      | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Select   | Details  | [PAS     |          |
|          |          | an       | shown    | S]{.stat |          |
|          |          | account. | will be  | us-macro |          |
|          |          |          | changed  | .aui     |          |
|          |          |          | to that  | -lozenge |          |
|          |          |          | of the   | .aui-    |          |
|          |          |          | selected | lozenge- |          |
|          |          |          | account. | success} |          |
+----------+----------+----------+----------+----------+----------+
| DASH-5   | N        | Click on | Shows    | [PAS     |          |
|          | amespace | "Na      | the      | S]{.stat |          |
|          |          | mespace" | a        | us-macro |          |
|          |          |          | vailable | .aui     |          |
|          |          |          | na       | -lozenge |          |
|          |          |          | mespaces | .aui-    |          |
|          |          |          | and      | lozenge- |          |
|          |          |          | their    | success} |          |
|          |          |          | details. |          |          |
+----------+----------+----------+----------+----------+----------+
| DASH-6   | Other    | Click on | Show the | [PAS     |          |
|          | Assets   | "Other   | a        | S]{.stat |          |
|          |          | Assets"  | vailable | us-macro |          |
|          |          |          | assets   | .aui     |          |
|          |          |          | and      | -lozenge |          |
|          |          |          | their    | .aui-    |          |
|          |          |          | details. | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| DASH-7   | Explorer | Click on | Goes to  | [PAS     |          |
|          |          | "E       | the      | S]{.stat |          |
|          |          | xplorer" | Explorer | us-macro |          |
|          |          | under    | page of  | .aui     |          |
|          |          | the      | the      | -lozenge |          |
|          |          | "Action" | specific | .aui-    |          |
|          |          | of any   | tran     | lozenge- |          |
|          |          | tran     | saction. | success} |          |
|          |          | saction. |          |          |          |
+----------+----------+----------+----------+----------+----------+
| DASH-8   | Sign out | Click on | Logs out | [PAS     |          |
|          |          | "Sign    | and      | S]{.stat |          |
|          |          | Out".    | r        | us-macro |          |
|          |          |          | edirects | .aui     |          |
|          |          |          | to the   | -lozenge |          |
|          |          |          | Home     | .aui-    |          |
|          |          |          | page.    | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
:::

::: table-wrap
+----------+----------+----------+----------+----------+----------+
| ## Tran  |          |          |          |          |          |
| sfer {#T |          |          |          |          |          |
| estCases |          |          |          |          |          |
| -0.0.7-T |          |          |          |          |          |
| ransfer} |          |          |          |          |          |
+----------+----------+----------+----------+----------+----------+
| **Test   | **Test   | **Test   | **       | **       | **R      |
| Case     | Sce      | steps**  | Expected | Status** | emarks** |
| ID**     | narios** |          | result** |          |          |
+----------+----------+----------+----------+----------+----------+
| TSFR-1   | Sender   | Observe  | Default  | [PAS     |          |
|          | account  | default  | account  | S]{.stat |          |
|          |          | value of | is being | us-macro |          |
|          |          | sender   | selected | .aui     |          |
|          |          | account  |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| TSFR-2   |          | Check if | Multisig | [NOT     |          |
|          |          | multisig | account  | READ     |          |
|          |          | account  | is shown | Y]{.stat |          |
|          |          | is shown | on drop  | us-macro |          |
|          |          | on drop  | down     | .aui-    |          |
|          |          | down     | list     | lozenge} |          |
|          |          | list     |          |          |          |
+----------+----------+----------+----------+----------+----------+
| TSFR-3   |          | Check if | Delegate | [PAS     |          |
|          |          | delegate | account  | S]{.stat |          |
|          |          | account  | is not   | us-macro |          |
|          |          | is shown | shown on | .aui     |          |
|          |          | on drop  | drop     | -lozenge |          |
|          |          | down     | down     | .aui-    |          |
|          |          | list     | list     | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| TSFR-4   |          | Select   | Cosigner | [NOT     |          |
|          |          | multisig | name and | READ     |          |
|          |          | account  | balance  | Y]{.stat |          |
|          |          | which    | is shown | us-macro |          |
|          |          | its      | below    | .aui-    |          |
|          |          | cosigner |          | lozenge} |          |
|          |          | is in    |          |          |          |
|          |          | this     |          |          |          |
|          |          | wallet   |          |          |          |
+----------+----------+----------+----------+----------+----------+
| TSFR-5   |          | If       | Shows    | [NOT     |          |
|          |          | co       | insu     | READ     |          |
|          |          | signer's | fficient | Y]{.stat |          |
|          |          | balance  | balance  | us-macro |          |
|          |          | is lower | error    | .aui-    |          |
|          |          | than     |          | lozenge} |          |
|          |          | lock     |          |          |          |
|          |          | fund     |          |          |          |
+----------+----------+----------+----------+----------+----------+
| TSFR-6   |          | Select   | No       | [NOT     |          |
|          |          | multisig | eligible | READ     |          |
|          |          | account  | cosigner | Y]{.stat |          |
|          |          | which    | error is | us-macro |          |
|          |          | its      | shown    | .aui-    |          |
|          |          | cosigner |          | lozenge} |          |
|          |          | is not   |          |          |          |
|          |          | in this  |          |          |          |
|          |          | wallet   |          |          |          |
+----------+----------+----------+----------+----------+----------+
| TSFR-7   | R        | Enter    | Invalid  | [PAS     |          |
|          | ecipient | invalid  | r        | S]{.stat |          |
|          |          | value on | ecipient | us-macro |          |
|          |          | r        | error is | .aui     |          |
|          |          | ecipient | shown    | -lozenge |          |
|          |          | field    |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| TSFR-8   |          | Click on | Contact  | [PAS     |          |
|          |          | contact  | list is  | S]{.stat |          |
|          |          | icon     | shown    | us-macro |          |
|          |          |          |          | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| TSFR-9   |          | Click on | Contact  | [PAS     |          |
|          |          | contact  | list is  | S]{.stat |          |
|          |          | icon     | hidden   | us-macro |          |
|          |          | again    |          | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| TSFR-10  |          | Click on | Owner's  | [NOT     |          |
|          |          | contact  | normal   | READ     |          |
|          |          | drop     | a        | Y]{.stat |          |
|          |          | down     | ccounts, | us-macro |          |
|          |          | list     | multisig | .aui-    |          |
|          |          |          | accounts | lozenge} |          |
|          |          |          | and      |          |          |
|          |          |          | contacts |          |          |
|          |          |          | are      |          |          |
|          |          |          | shown    |          |          |
+----------+----------+----------+----------+----------+----------+
| TSFR-11  | XPX      | Enter    | Shows    | [PAS     |          |
|          | amount   | invalid  | NaN      | S]{.stat |          |
|          |          | value    |          | us-macro |          |
|          |          |          |          | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| TSFR-12  |          | Balance  | Shows    | [PAS     |          |
|          |          | is less  | insu     | S]{.stat |          |
|          |          | than     | fficient | us-macro |          |
|          |          | tra      | balance  | .aui     |          |
|          |          | nsaction | error    | -lozenge |          |
|          |          | fee      |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| TSFR-13  |          | Entered  | Shows    | [PAS     |          |
|          |          | amount   | insu     | S]{.stat |          |
|          |          | is more  | fficient | us-macro |          |
|          |          | than     | balance  | .aui     |          |
|          |          | selected | error    | -lozenge |          |
|          |          | account  |          | .aui-    |          |
|          |          | balance  |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| TSFR-14  | Add      | Click    | Mosaic   | [PAS     |          |
|          | Mosaics  | add      | drop     | S]{.stat |          |
|          |          | mosaics  | down     | us-macro |          |
|          |          |          | list is  | .aui     |          |
|          |          |          | shown    | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| TSFR-15  |          | Select   | Shows    | [PAS     |          |
|          |          | mosaic   | asset id | S]{.stat |          |
|          |          |          | and      | us-macro |          |
|          |          |          | corre    | .aui     |          |
|          |          |          | sponding | -lozenge |          |
|          |          |          | balance  | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| TSFR-16  | Mosaic   | Entered  | Shows    | [NOT     |          |
|          | amount   | amount   | insu     | READ     |          |
|          |          | is more  | fficient | Y]{.stat |          |
|          |          | than     | balance  | us-macro |          |
|          |          | selected | error    | .aui-    |          |
|          |          | mosaic   |          | lozenge} |          |
|          |          | balance  |          |          |          |
+----------+----------+----------+----------+----------+----------+
| TSFR-17  | Regular  | Click on | Works    | [PAS     |          |
|          | /        | both     | properly | S]{.stat |          |
|          | Hex      | radio    |          | us-macro |          |
|          | adecimal | buttons  |          | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| TSFR-18  |          | Enter    | Allow    | [PAS     |          |
|          |          | message  | all      | S]{.stat |          |
|          |          | when     | inputs   | us-macro |          |
|          |          | regular  |          | .aui     |          |
|          |          | is       |          | -lozenge |          |
|          |          | selected |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| TSFR-19  |          | Enter    | Only     | [PAS     |          |
|          |          | message  | allow    | S]{.stat |          |
|          |          | when     | hex      | us-macro |          |
|          |          | hex      | adecimal | .aui     |          |
|          |          | adecimal | inputs   | -lozenge |          |
|          |          | is       |          | .aui-    |          |
|          |          | selected |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| TSFR-20  | E        | Click on | Works    | [PAS     |          |
|          | ncrypted | checkbox | properly | S]{.stat |          |
|          |          |          |          | us-macro |          |
|          |          |          |          | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| TSFR-21  | Message  | Enter    | E        | [PAS     |          |
|          |          | random   | ffective | S]{.stat |          |
|          |          | messages | Fee      | us-macro |          |
|          |          |          | i        | .aui     |          |
|          |          |          | ncreases | -lozenge |          |
|          |          |          | as       | .aui-    |          |
|          |          |          | message  | lozenge- |          |
|          |          |          | size     | success} |          |
|          |          |          | i        |          |          |
|          |          |          | ncreases |          |          |
+----------+----------+----------+----------+----------+----------+
| TSFR-22  |          | Enter    | Prevents | [NOT     |          |
|          |          | more     | input    | READ     |          |
|          |          | than     | upon     | Y]{.stat |          |
|          |          | maximum  | reaching | us-macro |          |
|          |          | of       | maximum  | .aui-    |          |
|          |          | message  | message  | lozenge} |          |
|          |          | limit    | limit    |          |          |
+----------+----------+----------+----------+----------+----------+
| TSFR-23  | Password | Leave    | Displays | [PAS     |          |
|          |          | password | please   | S]{.stat |          |
|          |          | empty    | enter    | us-macro |          |
|          |          |          | wallet   | .aui     |          |
|          |          |          | password | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| TSFR-24  | Clear    | Click on | Sender,  | [PAS     |          |
|          |          | clear    | re       | S]{.stat |          |
|          |          |          | cipient, | us-macro |          |
|          |          |          | send     | .aui     |          |
|          |          |          | amount,  | -lozenge |          |
|          |          |          | mosaic   | .aui-    |          |
|          |          |          | amount,  | lozenge- |          |
|          |          |          | message  | success} |          |
|          |          |          | and      |          |          |
|          |          |          | password |          |          |
|          |          |          | fields   |          |          |
|          |          |          | reset to |          |          |
|          |          |          | default  |          |          |
+----------+----------+----------+----------+----------+----------+
| TSFR-25  | Create   | Click    | Transfer | [PAS     |          |
|          |          | create   | tra      | S]{.stat |          |
|          |          | when     | nsaction | us-macro |          |
|          |          | there    | is       | .aui     |          |
|          |          | are at   | succ     | -lozenge |          |
|          |          | least    | essfully | .aui-    |          |
|          |          | r        | created  | lozenge- |          |
|          |          | ecipient |          | success} |          |
|          |          | and      |          |          |          |
|          |          | password |          |          |          |
|          |          | field    |          |          |          |
|          |          | filled   |          |          |          |
|          |          | in       |          |          |          |
+----------+----------+----------+----------+----------+----------+
| TSFR-26  |          | Click    | Create   | [PAS     |          |
|          |          | create   | button   | S]{.stat |          |
|          |          | when any | is       | us-macro |          |
|          |          | of the   | disabled | .aui     |          |
|          |          | above    |          | -lozenge |          |
|          |          | fields   |          | .aui-    |          |
|          |          | are      |          | lozenge- |          |
|          |          | empty    |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| TSFR-27  |          | Create   | Transfer | [PAS     |          |
|          |          | transfer | tra      | S]{.stat |          |
|          |          | with     | nsaction | us-macro |          |
|          |          | multisig | is       | .aui     |          |
|          |          | account  | succ     | -lozenge |          |
|          |          |          | essfully | .aui-    |          |
|          |          |          | created  | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| TSFR-28  |          | Create   | Transfer | [PAS     |          |
|          |          | transfer | tra      | S]{.stat |          |
|          |          | with     | nsaction | us-macro |          |
|          |          | normal   | is       | .aui     |          |
|          |          | account  | succ     | -lozenge |          |
|          |          |          | essfully | .aui-    |          |
|          |          |          | created  | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| TSFR-29  |          | Create   | Shows    | [PAS     |          |
|          |          | any      | password | S]{.stat |          |
|          |          | transfer | invalid  | us-macro |          |
|          |          | with     | error    | .aui     |          |
|          |          | wrong    |          | -lozenge |          |
|          |          | password |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
:::

::: table-wrap
+----------+----------+----------+----------+----------+----------+
| ## Acco  |          |          |          |          |          |
| unts {#T |          |          |          |          |          |
| estCases |          |          |          |          |          |
| -0.0.7-A |          |          |          |          |          |
| ccounts} |          |          |          |          |          |
+----------+----------+----------+----------+----------+----------+
| **Test   | **Test   | **Test   | **       | **       | **R      |
| Case     | Sce      | steps**  | Expected | Status** | emarks** |
| ID**     | narios** |          | result** |          |          |
+----------+----------+----------+----------+----------+----------+
| #### C   |          |          |          |          |          |
| reate a  |          |          |          |          |          |
| New Acco |          |          |          |          |          |
| unt {#Te |          |          |          |          |          |
| stCases- |          |          |          |          |          |
| 0.0.7-Cr |          |          |          |          |          |
| eateaNew |          |          |          |          |          |
| Account} |          |          |          |          |          |
+----------+----------+----------+----------+----------+----------+
| ACCTS-1  | Create a | Click    | Go to    | [PAS     |          |
|          | New      | "Create  | "Account | S]{.stat |          |
|          | Account  | a New    | \>       | us-macro |          |
|          | (P       | Account" | Select   | .aui     |          |
|          | ositive) |          | Creation | -lozenge |          |
|          |          |          | Type"    | .aui-    |          |
|          |          |          | Page     | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click    | Go to    | [PAS     |          |
|          |          | "New"    | "Account | S]{.stat |          |
|          |          |          | \>       | us-macro |          |
|          |          |          | Create   | .aui     |          |
|          |          |          | New      | -lozenge |          |
|          |          |          | Account" | .aui-    |          |
|          |          |          | Page     | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Enter    | Accepts  | [PAS     |          |
|          |          | Account  | the      | S]{.stat |          |
|          |          | Name     | input.   | us-macro |          |
|          |          |          | No error | .aui     |          |
|          |          |          | message  | -lozenge |          |
|          |          |          | is       | .aui-    |          |
|          |          |          | shown.   | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Enter    | Accepts  | [PAS     |          |
|          |          | valid    | the      | S]{.stat |          |
|          |          | wallet   | input.   | us-macro |          |
|          |          | password | No error | .aui     |          |
|          |          |          | message  | -lozenge |          |
|          |          |          | is       | .aui-    |          |
|          |          |          | shown.   | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click    | Account  | [PAS     |          |
|          |          | "Create" | created. | S]{.stat |          |
|          |          |          |          | us-macro |          |
|          |          |          |          | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| ACCTS-2  | Create a | Click    | Go to    | [PAS     |          |
|          | New      | "Create  | "Account | S]{.stat |          |
|          | Account  | a New    | \>       | us-macro |          |
|          | (N       | Account" | Select   | .aui     |          |
|          | egative) |          | Creation | -lozenge |          |
|          |          |          | Type"    | .aui-    |          |
|          |          |          | Page     | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click    | Go to    | [PAS     |          |
|          |          | "New"    | "Account | S]{.stat |          |
|          |          |          | \>       | us-macro |          |
|          |          |          | Create   | .aui     |          |
|          |          |          | New      | -lozenge |          |
|          |          |          | Account" | .aui-    |          |
|          |          |          | Page     | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Enter    | Accepts  | [PAS     |          |
|          |          | Account  | the      | S]{.stat |          |
|          |          | Name     | input.   | us-macro |          |
|          |          |          | No error | .aui     |          |
|          |          |          | message  | -lozenge |          |
|          |          |          | is       | .aui-    |          |
|          |          |          | shown.   | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Enter    | No error | [PAS     |          |
|          |          | invalid  | message  | S]{.stat |          |
|          |          | wallet   | is       | us-macro |          |
|          |          | password | shown.   | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click    | Invalid  | [PAS     |          |
|          |          | "Create" | password | S]{.stat |          |
|          |          |          | message  | us-macro |          |
|          |          |          | is       | .aui     |          |
|          |          |          | shown.   | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| ACCTS-2  | Account  | Click on | Goes to  | [PAS     |          |
|          | Details  | "A       | "Account | S]{.stat |          |
|          |          | ccounts" | \> View  | us-macro |          |
|          |          | tab in   | All"     | .aui     |          |
|          |          | the home | page     | -lozenge |          |
|          |          | page.    |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | Shows a  | [PAS     |          |
|          |          | the      | dropdown | S]{.stat |          |
|          |          | arrow    | list of  | us-macro |          |
|          |          | button   | viable   | .aui     |          |
|          |          | on one   | options  | -lozenge |          |
|          |          | of the   |          | .aui-    |          |
|          |          | a        |          | lozenge- |          |
|          |          | vailable |          | success} |          |
|          |          | accounts |          |          |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | Goes to  | [PAS     |          |
|          |          | "        | "Account | S]{.stat |          |
|          |          | Details" | \>       | us-macro |          |
|          |          |          | Details" | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| ACCTS-3  | Make     | Click on | Goes to  | [PAS     |          |
|          | Default  | "A       | "Account | S]{.stat |          |
|          |          | ccounts" | \> View  | us-macro |          |
|          |          | tab in   | All"     | .aui     |          |
|          |          | the home | page     | -lozenge |          |
|          |          | page.    |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | Shows a  | [PAS     |          |
|          |          | the      | dropdown | S]{.stat |          |
|          |          | arrow    | list of  | us-macro |          |
|          |          | button   | viable   | .aui     |          |
|          |          | on one   | options  | -lozenge |          |
|          |          | of the   |          | .aui-    |          |
|          |          | a        |          | lozenge- |          |
|          |          | vailable |          | success} |          |
|          |          | accounts |          |          |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | "        | [PAS     |          |
|          |          | "Make    | Default" | S]{.stat |          |
|          |          | Default" | is shown | us-macro |          |
|          |          |          | beside   | .aui     |          |
|          |          |          | account  | -lozenge |          |
|          |          |          | name     | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| ACCTS-4  | Export   | Click on | Goes to  | [PAS     |          |
|          |          | "A       | "Account | S]{.stat |          |
|          |          | ccounts" | \> View  | us-macro |          |
|          |          | tab in   | All"     | .aui     |          |
|          |          | the home | page     | -lozenge |          |
|          |          | page.    |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | Shows a  | [PAS     |          |
|          |          | the      | dropdown | S]{.stat |          |
|          |          | arrow    | list of  | us-macro |          |
|          |          | button   | viable   | .aui     |          |
|          |          | on one   | options  | -lozenge |          |
|          |          | of the   |          | .aui-    |          |
|          |          | a        |          | lozenge- |          |
|          |          | vailable |          | success} |          |
|          |          | accounts |          |          |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | The      | [PAS     |          |
|          |          | "Export" | account  | S]{.stat |          |
|          |          |          | will be  | us-macro |          |
|          |          |          | do       | .aui     |          |
|          |          |          | wnloaded | -lozenge |          |
|          |          |          | into     | .aui-    |          |
|          |          |          | local    | lozenge- |          |
|          |          |          | machine  | success} |          |
|          |          |          | in .wlt  |          |          |
|          |          |          | file     |          |          |
|          |          |          | format   |          |          |
+----------+----------+----------+----------+----------+----------+
| ACCTS-5  | Delete   | Click on | Goes to  | [PAS     |          |
|          |          | "A       | "Account | S]{.stat |          |
|          |          | ccounts" | \> View  | us-macro |          |
|          |          | tab in   | All"     | .aui     |          |
|          |          | the home | page     | -lozenge |          |
|          |          | page.    |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | Shows a  | [PAS     |          |
|          |          | the      | dropdown | S]{.stat |          |
|          |          | arrow    | list of  | us-macro |          |
|          |          | button   | viable   | .aui     |          |
|          |          | on one   | options  | -lozenge |          |
|          |          | of the   |          | .aui-    |          |
|          |          | a        |          | lozenge- |          |
|          |          | vailable |          | success} |          |
|          |          | accounts |          |          |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | Goes to  | [PAS     |          |
|          |          | "Delete" | "        | S]{.stat |          |
|          |          |          | Accounts | us-macro |          |
|          |          |          | \>       | .aui     |          |
|          |          |          | Delete"  | -lozenge |          |
|          |          |          | page     | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | Shows    | [PAS     |          |
|          |          | "        | warning  | S]{.stat |          |
|          |          | Proceed" | message  | us-macro |          |
|          |          |          |          | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | The      | [PAS     |          |
|          |          | the "I   | checkbox | S]{.stat |          |
|          |          | have     | is       | us-macro |          |
|          |          | read the | ticked   | .aui     |          |
|          |          | warning" |          | -lozenge |          |
|          |          | checkbox |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | Account  | [PAS     |          |
|          |          | "Delete  | is       | S]{.stat |          |
|          |          | now"     | deleted  | us-macro |          |
|          |          |          |          | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          | Multisig |          | Go to    | [NOT     |          |
|          |          |          | "        | READ     |          |
|          |          |          | Accounts | Y]{.stat |          |
|          |          |          | \>       | us-macro |          |
|          |          |          | Multisig | .aui-    |          |
|          |          |          | \>       | lozenge} |          |
|          |          |          | Convert  |          |          |
|          |          |          | to       |          |          |
|          |          |          | Multisig |          |          |
|          |          |          | Account" |          |          |
+----------+----------+----------+----------+----------+----------+
|          | Rest     |          |          | [NOT     |          |
|          | rictions |          |          | READ     |          |
|          |          |          |          | Y]{.stat |          |
|          |          |          |          | us-macro |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge} |          |
+----------+----------+----------+----------+----------+----------+
|          | Metadata |          |          | [NOT     |          |
|          |          |          |          | READ     |          |
|          |          |          |          | Y]{.stat |          |
|          |          |          |          | us-macro |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge} |          |
+----------+----------+----------+----------+----------+----------+
| ACCTS-6  | Delegate | Click on | Goes to  | [PAS     |          |
|          |          | "A       | "Account | S]{.stat |          |
|          |          | ccounts" | \> View  | us-macro |          |
|          |          | tab in   | All"     | .aui     |          |
|          |          | the home | page     | -lozenge |          |
|          |          | page.    |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | Shows a  | [PAS     |          |
|          |          | the      | dropdown | S]{.stat |          |
|          |          | arrow    | list of  | us-macro |          |
|          |          | button   | viable   | .aui     |          |
|          |          | on one   | options  | -lozenge |          |
|          |          | of the   |          | .aui-    |          |
|          |          | a        |          | lozenge- |          |
|          |          | vailable |          | success} |          |
|          |          | accounts |          |          |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | Goes to  | [PAS     |          |
|          |          | "D       | "        | S]{.stat |          |
|          |          | elegate" | Accounts | us-macro |          |
|          |          |          | \>       | .aui     |          |
|          |          |          | D        | -lozenge |          |
|          |          |          | elegate" | .aui-    |          |
|          |          |          | page     | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | "Select  | [PAS     |          |
|          |          | the edit | Account  | S]{.stat |          |
|          |          | icon     | Type"    | us-macro |          |
|          |          |          | pops up  | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | "New     | [PAS     |          |
|          |          | "Select" | Account" | S]{.stat |          |
|          |          | under    | is shown | us-macro |          |
|          |          | "New     | under    | .aui     |          |
|          |          | Account" | "Linking | -lozenge |          |
|          |          |          | A        | .aui-    |          |
|          |          |          | ccount:" | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Enter    | No error | [PAS     |          |
|          |          | valid    | message  | S]{.stat |          |
|          |          | wallet   | is shown | us-macro |          |
|          |          | Password |          | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | Delegate | [PAS     |          |
|          |          | "Link    | account  | S]{.stat |          |
|          |          | New      | is       | us-macro |          |
|          |          | Account" | created  | .aui     |          |
|          |          |          | and      | -lozenge |          |
|          |          |          | linked   | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| ACCTS-7  | Link to  | Click on | Goes to  | [PAS     |          |
|          | N        | "A       | "Account | S]{.stat |          |
|          | amespace | ccounts" | \> View  | us-macro |          |
|          |          | tab in   | All"     | .aui     |          |
|          |          | the home | page     | -lozenge |          |
|          |          | page.    |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | Shows a  | [PAS     |          |
|          |          | the      | dropdown | S]{.stat |          |
|          |          | arrow    | list of  | us-macro |          |
|          |          | button   | viable   | .aui     |          |
|          |          | on one   | options  | -lozenge |          |
|          |          | of the   |          | .aui-    |          |
|          |          | a        |          | lozenge- |          |
|          |          | vailable |          | success} |          |
|          |          | accounts |          |          |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | Goes to  | [PAS     |          |
|          |          | "Link to | "        | S]{.stat |          |
|          |          | Na       | Accounts | us-macro |          |
|          |          | mespace" | \> Link  | .aui     |          |
|          |          |          | to       | -lozenge |          |
|          |          |          | Na       | .aui-    |          |
|          |          |          | mespace" | lozenge- |          |
|          |          |          | page     | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | Show a   | [PAS     |          |
|          |          | "Link"   | list of  | S]{.stat |          |
|          |          | under    | "Link"   | us-macro |          |
|          |          | "Select  | and      | .aui     |          |
|          |          | action". | "        | -lozenge |          |
|          |          |          | Unlink". | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Select   | Shows    | [PAS     |          |
|          |          | "Link".  | that     | S]{.stat |          |
|          |          |          | "Link"   | us-macro |          |
|          |          |          | is       | .aui     |          |
|          |          |          | s        | -lozenge |          |
|          |          |          | elected. | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | Show a   | [PAS     |          |
|          |          | "Select  | list of  | S]{.stat |          |
|          |          | na       | a        | us-macro |          |
|          |          | mespace" | vailable | .aui     |          |
|          |          | under    | nam      | -lozenge |          |
|          |          | "Select  | espaces. | .aui-    |          |
|          |          | nam      |          | lozenge- |          |
|          |          | espace". |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Select   | Shows    | [PAS     |          |
|          |          | one of   | that the | S]{.stat |          |
|          |          | the      | n        | us-macro |          |
|          |          | a        | amespace | .aui     |          |
|          |          | vailable | is       | -lozenge |          |
|          |          | nam      | s        | .aui-    |          |
|          |          | espaces. | elected. | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Enter a  | No       | [PAS     |          |
|          |          | valid    | message  | S]{.stat |          |
|          |          | address  | is       | us-macro |          |
|          |          | in the   | shown.   | .aui     |          |
|          |          | "        |          | -lozenge |          |
|          |          | Address" |          | .aui-    |          |
|          |          | input    |          | lozenge- |          |
|          |          | field.   |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Enter    | No       | [PAS     |          |
|          |          | the      | message  | S]{.stat |          |
|          |          | valid    | is       | us-macro |          |
|          |          | wallet   | shown.   | .aui     |          |
|          |          | password |          | -lozenge |          |
|          |          | in the   |          | .aui-    |          |
|          |          | "Enter   |          | lozenge- |          |
|          |          | wallet   |          | success} |          |
|          |          | pa       |          |          |          |
|          |          | ssword". |          |          |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | N        | [PAS     |          |
|          |          | "        | amespace | S]{.stat |          |
|          |          | Create". | is       | us-macro |          |
|          |          |          | linked   | .aui     |          |
|          |          |          | to the   | -lozenge |          |
|          |          |          | selected | .aui-    |          |
|          |          |          | account. | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| ### Se   |          |          |          |          |          |
| lect Cre |          |          |          |          |          |
| ation Ty |          |          |          |          |          |
| pe {#Tes |          |          |          |          |          |
| tCases-0 |          |          |          |          |          |
| .0.7-Sel |          |          |          |          |          |
| ectCreat |          |          |          |          |          |
| ionType} |          |          |          |          |          |
+----------+----------+----------+----------+----------+----------+
| NEWACC-1 | New      | Click on | Go to    | [PAS     |          |
|          |          | "New"    | "Create  | S]{.stat |          |
|          |          | button   | a New    | us-macro |          |
|          |          |          | Account  | .aui     |          |
|          |          |          | Page     | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| NEWACC-2 | From a   | Click on | Go to    | [PAS     |          |
|          | Private  | "From a  | "Import  | S]{.stat |          |
|          | Key      | Private  | Account" | us-macro |          |
|          |          | Key"     | Page     | .aui     |          |
|          |          | button   |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| ####     |          |          |          |          |          |
|  Import  |          |          |          |          |          |
| Account  |          |          |          |          |          |
| {#TestCa |          |          |          |          |          |
| ses-0.0. |          |          |          |          |          |
| 7-Import |          |          |          |          |          |
| Account} |          |          |          |          |          |
+----------+----------+----------+----------+----------+----------+
| IMPACC-1 | Import   | Click on | Go to    | [PAS     |          |
|          | Account  | "A       | "Account | S]{.stat |          |
|          |          | ccounts" | \> View  | us-macro |          |
|          |          | tab on   | All"     | .aui     |          |
|          |          | the home | page.    | -lozenge |          |
|          |          | page     |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | Go to    | [PAS     |          |
|          |          | "Create  | "        | S]{.stat |          |
|          |          | a New    | Accounts | us-macro |          |
|          |          | Account" | \>       | .aui     |          |
|          |          |          | Select   | -lozenge |          |
|          |          |          | Creation | .aui-    |          |
|          |          |          | Type"    | lozenge- |          |
|          |          |          | page.    | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | Go to    | [PAS     |          |
|          |          | "From a  | "Ac      | S]{.stat |          |
|          |          | Private  | counts\> | us-macro |          |
|          |          | Key"     | Import   | .aui     |          |
|          |          |          | Account" | -lozenge |          |
|          |          |          | page.    | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Enter    | No error | [PAS     |          |
|          |          | valid    | message  | S]{.stat |          |
|          |          | private  | is       | us-macro |          |
|          |          | key      | shown.   | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | The      | [PAS     |          |
|          |          | the      | checkbox | S]{.stat |          |
|          |          | "Check   | is       | us-macro |          |
|          |          | this     | ticked.  | .aui     |          |
|          |          | box..."  |          | -lozenge |          |
|          |          | checkbox |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Enter    | No error | [PAS     |          |
|          |          | account  | message  | S]{.stat |          |
|          |          | name     | is       | us-macro |          |
|          |          |          | shown.   | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Enter    | No error | [PAS     |          |
|          |          | valid    | message  | S]{.stat |          |
|          |          | wallet   | is       | us-macro |          |
|          |          | password | shown.   | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | Account  | [PAS     |          |
|          |          | "Import" | is       | S]{.stat |          |
|          |          |          | created. | us-macro |          |
|          |          |          |          | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| ### E    |          |          |          |          |          |
| dit an e |          |          |          |          |          |
| xisting  |          |          |          |          |          |
| Account  |          |          |          |          |          |
| {#TestCa |          |          |          |          |          |
| ses-0.0. |          |          |          |          |          |
| 7-Editan |          |          |          |          |          |
| existing |          |          |          |          |          |
| Account} |          |          |          |          |          |
+----------+----------+----------+----------+----------+----------+
| #### De  |          |          |          |          |          |
| tails {# |          |          |          |          |          |
| TestCase |          |          |          |          |          |
| s-0.0.7- |          |          |          |          |          |
| Details} |          |          |          |          |          |
+----------+----------+----------+----------+----------+----------+
| ACCD     | Change   | Click on | Shows an | [PAS     |          |
| ETAILS-1 | "Account | edit     | input    | S]{.stat |          |
|          | Name"    | icon in  | field    | us-macro |          |
|          |          | the      | with     | .aui     |          |
|          |          | "Account | account  | -lozenge |          |
|          |          | Name"    | name     | .aui-    |          |
|          |          | box      | inside.  | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Change   | No       | [PAS     |          |
|          |          | the      | message  | S]{.stat |          |
|          |          | account  | is       | us-macro |          |
|          |          | name     | shown.   | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | The      | [PAS     |          |
|          |          | "![(blue | input    | S]{.stat |          |
|          |          | star     | field    | us-macro |          |
|          |          | )](image | di       | .aui     |          |
|          |          | s/icons/ | sappears | -lozenge |          |
|          |          | emoticon | and      | .aui-    |          |
|          |          | s/72/271 | shows    | lozenge- |          |
|          |          | 4.png){. | the      | success} |          |
|          |          | emoticon | changed  |          |          |
|          |          | .em      | account  |          |          |
|          |          | oticon-b | name.    |          |          |
|          |          | lue-star |          |          |          |
|          |          | emoji-i  |          |          |          |
|          |          | d="2714" |          |          |          |
|          |          | emoj     |          |          |          |
|          |          | i-shortn |          |          |          |
|          |          | ame=":he |          |          |          |
|          |          | avy_chec |          |          |          |
|          |          | k_mark:" |          |          |          |
|          |          | em       |          |          |          |
|          |          | oji-fall |          |          |          |
|          |          | back="✔" |          |          |          |
|          |          | wi       |          |          |          |
|          |          | dth="16" |          |          |          |
|          |          | hei      |          |          |          |
|          |          | ght="16" |          |          |          |
|          |          | emo      |          |          |          |
|          |          | ticon-na |          |          |          |
|          |          | me="blue |          |          |          |
|          |          | -star"}" |          |          |          |
+----------+----------+----------+----------+----------+----------+
| ACCD     | Copy     | Click    | Address  | [PAS     |          |
| ETAILS-2 | "        | "Copy"   | is       | S]{.stat |          |
|          | Address" | icon in  | copied.  | us-macro |          |
|          |          | Address  |          | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| ACCD     | Copy     | Click    | Public   | [PAS     |          |
| ETAILS-3 | "Public  | "Copy"   | key is   | S]{.stat |          |
|          | Key"     | icon in  | copied   | us-macro |          |
|          |          | Public   |          | .aui     |          |
|          |          | Key      |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| ACCD     | Show     | Click    | Shows an | [PAS     |          |
| ETAILS-4 | "Private | "Show"   | input    | S]{.stat |          |
|          | Key"     | in       | field .  | us-macro |          |
|          |          | Private  |          | .aui     |          |
|          |          | Key\     |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Enter    | Private  | [PAS     |          |
|          |          | correct  | key is   | S]{.stat |          |
|          |          | wallet   | shown.   | us-macro |          |
|          |          | p        |          | .aui     |          |
|          |          | assword\ |          | -lozenge |          |
|          |          | Click    |          | .aui-    |          |
|          |          | "Submit" |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Enter    | Shows    | [PAS     |          |
|          |          | i        | error    | S]{.stat |          |
|          |          | ncorrect | message  | us-macro |          |
|          |          | wallet   |          | .aui     |          |
|          |          | p        |          | -lozenge |          |
|          |          | assword\ |          | .aui-    |          |
|          |          | Click    |          | lozenge- |          |
|          |          | "Submit" |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Enter    | Shows    | [PAS     |          |
|          |          | blank    | error    | S]{.stat |          |
|          |          | wallet   | message. | us-macro |          |
|          |          | p        |          | .aui     |          |
|          |          | assword\ |          | -lozenge |          |
|          |          | Click    |          | .aui-    |          |
|          |          | "Submit" |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| ACCD     | Swap     | Click    |          | [NOT     |          |
| ETAILS-5 | with     | "Enable" |          | READ     |          |
|          | this     | in Swap  |          | Y]{.stat |          |
|          | private  | with     |          | us-macro |          |
|          | key      | this     |          | .aui-    |          |
|          |          | private  |          | lozenge} |          |
|          |          | key      |          |          |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Enter    |          | [NOT     |          |
|          |          | correct  |          | READ     |          |
|          |          | wallet   |          | Y]{.stat |          |
|          |          | p        |          | us-macro |          |
|          |          | assword\ |          | .aui-    |          |
|          |          | Click    |          | lozenge} |          |
|          |          | Submit   |          |          |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Enter    |          | [NOT     |          |
|          |          | i        |          | READ     |          |
|          |          | ncorrect |          | Y]{.stat |          |
|          |          | wallet   |          | us-macro |          |
|          |          | p        |          | .aui-    |          |
|          |          | assword\ |          | lozenge} |          |
|          |          | Click    |          |          |          |
|          |          | Submit   |          |          |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Enter    |          | [NOT     |          |
|          |          | blank    |          | READ     |          |
|          |          | wallet   |          | Y]{.stat |          |
|          |          | p        |          | us-macro |          |
|          |          | assword\ |          | .aui-    |          |
|          |          | Click    |          | lozenge} |          |
|          |          | Submit   |          |          |          |
+----------+----------+----------+----------+----------+----------+
| ACCD     | Save as  | Click    | Shows an | [PAS     |          |
| ETAILS-6 | paper    | "Save in | input    | S]{.stat |          |
|          | wallet   | Save as  | field.   | us-macro |          |
|          |          | wallet   |          | .aui     |          |
|          |          | paper    |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Enter    | Wallet   | [PAS     |          |
|          |          | correct  | is       | S]{.stat |          |
|          |          | wallet   | do       | us-macro |          |
|          |          | p        | wnloaded | .aui     |          |
|          |          | assword\ | as PDF   | -lozenge |          |
|          |          | Click    | file to  | .aui-    |          |
|          |          | Submit   | local    | lozenge- |          |
|          |          |          | machine  | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Enter    | Error    | [PAS     |          |
|          |          | i        | message  | S]{.stat |          |
|          |          | ncorrect | is       | us-macro |          |
|          |          | wallet   | shown.   | .aui     |          |
|          |          | p        |          | -lozenge |          |
|          |          | assword\ |          | .aui-    |          |
|          |          | Click    |          | lozenge- |          |
|          |          | Submit   |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Enter    | Shows    | [PAS     |          |
|          |          | blank    | error    | S]{.stat |          |
|          |          | wallet   | message. | us-macro |          |
|          |          | p        |          | .aui     |          |
|          |          | assword\ |          | -lozenge |          |
|          |          | Click    |          | .aui-    |          |
|          |          | Submit   |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| ###      |          |          |          |          |          |
| Convert  |          |          |          |          |          |
| to Multi |          |          |          |          |          |
| sig {#Te |          |          |          |          |          |
| stCases- |          |          |          |          |          |
| 0.0.7-Co |          |          |          |          |          |
| nverttoM |          |          |          |          |          |
| ultisig} |          |          |          |          |          |
+----------+----------+----------+----------+----------+----------+
| C        | Scheme   | Add and  | Value    | [NOT     |          |
| VTMTSG-1 |          | reduce   | does not | READ     |          |
|          |          | approve  | exceed   | Y]{.stat |          |
|          |          | tran     | max      | us-macro |          |
|          |          | sactions | number   | .aui-    |          |
|          |          |          | of       | lozenge} |          |
|          |          |          | cosig    |          |          |
|          |          |          | natories |          |          |
+----------+----------+----------+----------+----------+----------+
| C        |          | Add and  | Value    | [NOT     |          |
| VTMTSG-2 |          | reduce   | does not | READ     |          |
|          |          | delete   | exceed   | Y]{.stat |          |
|          |          | users    | max      | us-macro |          |
|          |          |          | number   | .aui-    |          |
|          |          |          | of       | lozenge} |          |
|          |          |          | cosig    |          |          |
|          |          |          | natories |          |          |
+----------+----------+----------+----------+----------+----------+
| C        | Add      | Click    | Opens up | [NOT     |          |
| VTMTSG-3 | Cos      | Add      | cos      | READ     |          |
|          | ignatory | Cos      | ignatory | Y]{.stat |          |
|          |          | ignatory | public   | us-macro |          |
|          |          |          | key      | .aui-    |          |
|          |          |          | field    | lozenge} |          |
+----------+----------+----------+----------+----------+----------+
| C        |          | Input    | Shows    | [NOT     |          |
| VTMTSG-4 |          | invalid  | invalid  | READ     |          |
|          |          | public   | public   | Y]{.stat |          |
|          |          | key      | key      | us-macro |          |
|          |          |          | error    | .aui-    |          |
|          |          |          |          | lozenge} |          |
+----------+----------+----------+----------+----------+----------+
| C        |          | Click on | Shows    | [NOT     |          |
| VTMTSG-5 |          | contact  | all      | READ     |          |
|          |          | icon     | normal   | Y]{.stat |          |
|          |          |          | accounts | us-macro |          |
|          |          |          | and      | .aui-    |          |
|          |          |          | contacts | lozenge} |          |
|          |          |          | a        |          |          |
|          |          |          | vailable |          |          |
+----------+----------+----------+----------+----------+----------+
| C        | Password | Leave    | Displays | [NOT     |          |
| VTMTSG-6 |          | password | password | READ     |          |
|          |          | field    | is       | Y]{.stat |          |
|          |          | empty    | required | us-macro |          |
|          |          |          | error    | .aui-    |          |
|          |          |          |          | lozenge} |          |
+----------+----------+----------+----------+----------+----------+
| C        | Clear    | Click    | Scheme,  | [NOT     |          |
| VTMTSG-7 |          | clear    | Added    | READ     |          |
|          |          |          | Cos      | Y]{.stat |          |
|          |          |          | ignatory | us-macro |          |
|          |          |          | and      | .aui-    |          |
|          |          |          | password | lozenge} |          |
|          |          |          | field    |          |          |
|          |          |          | are      |          |          |
|          |          |          | reset to |          |          |
|          |          |          | default  |          |          |
+----------+----------+----------+----------+----------+----------+
| C        | Send     | Click    | Converts | [NOT     |          |
| VTMTSG-8 |          | send     | account  | READ     |          |
|          |          | when     | to       | Y]{.stat |          |
|          |          | there is | multisig | us-macro |          |
|          |          | at least |          | .aui-    |          |
|          |          | one      |          | lozenge} |          |
|          |          | cos      |          |          |          |
|          |          | ignatory |          |          |          |
|          |          | added    |          |          |          |
|          |          | and      |          |          |          |
|          |          | password |          |          |          |
|          |          | field is |          |          |          |
|          |          | filled   |          |          |          |
+----------+----------+----------+----------+----------+----------+
| C        |          | Click    | Send     | [NOT     |          |
| VTMTSG-9 |          | send     | button   | READ     |          |
|          |          | when     | is       | Y]{.stat |          |
|          |          | scheme   | disabled | us-macro |          |
|          |          | values   |          | .aui-    |          |
|          |          | are      |          | lozenge} |          |
|          |          | adjusted |          |          |          |
|          |          | to 0     |          |          |          |
+----------+----------+----------+----------+----------+----------+
| CV       |          | Click    | Send     | [NOT     |          |
| TMTSG-10 |          | send     | button   | READ     |          |
|          |          | when any | is       | Y]{.stat |          |
|          |          | of the   | disabled | us-macro |          |
|          |          | above    |          | .aui-    |          |
|          |          | are not  |          | lozenge} |          |
|          |          | f        |          |          |          |
|          |          | ulfilled |          |          |          |
+----------+----------+----------+----------+----------+----------+
| CV       |          | Click    | Displays | [NOT     |          |
| TMTSG-11 |          | send     | password | READ     |          |
|          |          | when     | invalid  | Y]{.stat |          |
|          |          | password | error    | us-macro |          |
|          |          | is       |          | .aui-    |          |
|          |          | invalid  |          | lozenge} |          |
+----------+----------+----------+----------+----------+----------+
| #        |          |          |          |          |          |
| ## Edit  |          |          |          |          |          |
| Multisig |          |          |          |          |          |
|  {#TestC |          |          |          |          |          |
| ases-0.0 |          |          |          |          |          |
| .7-EditM |          |          |          |          |          |
| ultisig} |          |          |          |          |          |
+----------+----------+----------+----------+----------+----------+
| E        | Multisig | Click    | Multisig | [NOT     |          |
| DTMTSG-1 | Graph    | branch   | graph is | READ     |          |
|          |          | icon     | d        | Y]{.stat |          |
|          |          |          | isplayed | us-macro |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge} |          |
+----------+----------+----------+----------+----------+----------+
| E        | Remove   | Click on | Cosig    | [NOT     |          |
| DTMTSG-2 | cos      | drop     | natories | READ     |          |
|          | ignatory | down     | are      | Y]{.stat |          |
|          |          | icon     | d        | us-macro |          |
|          |          |          | isplayed | .aui-    |          |
|          |          |          |          | lozenge} |          |
+----------+----------+----------+----------+----------+----------+
| E        |          | Click on | Selected | [NOT     |          |
| DTMTSG-3 |          | delete   | cosigner | READ     |          |
|          |          | icon     | is       | Y]{.stat |          |
|          |          |          | hig      | us-macro |          |
|          |          |          | hlighted | .aui-    |          |
|          |          |          | as       | lozenge} |          |
|          |          |          | removing | [NOT     |          |
|          |          |          |          | READ     |          |
|          |          |          |          | Y]{.stat |          |
|          |          |          |          | us-macro |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge} |          |
+----------+----------+----------+----------+----------+----------+
| E        | Add      | Click    | Opens up | [NOT     |          |
| DTMTSG-4 | Cos      | Add      | cos      | READ     |          |
|          | ignatory | Cos      | ignatory | Y]{.stat |          |
|          |          | ignatory | public   | us-macro |          |
|          |          |          | key      | .aui-    |          |
|          |          |          | field    | lozenge} |          |
+----------+----------+----------+----------+----------+----------+
| E        |          | Input    | Shows    | [NOT     |          |
| DTMTSG-5 |          | invalid  | invalid  | READ     |          |
|          |          | public   | public   | Y]{.stat |          |
|          |          | key      | key      | us-macro |          |
|          |          |          | error    | .aui-    |          |
|          |          |          |          | lozenge} |          |
+----------+----------+----------+----------+----------+----------+
| E        |          | Click on | Shows    | [NOT     |          |
| DTMTSG-6 |          | contact  | all      | READ     |          |
|          |          | icon     | normal   | Y]{.stat |          |
|          |          |          | accounts | us-macro |          |
|          |          |          | and      | .aui-    |          |
|          |          |          | contacts | lozenge} |          |
|          |          |          | a        |          |          |
|          |          |          | vailable |          |          |
+----------+----------+----------+----------+----------+----------+
| E        | Scheme   | Add and  | Value    | [NOT     |          |
| DTMTSG-7 |          | reduce   | does not | READ     |          |
|          |          | approve  | exceed   | Y]{.stat |          |
|          |          | tran     | max      | us-macro |          |
|          |          | sactions | number   | .aui-    |          |
|          |          |          | of       | lozenge} |          |
|          |          |          | cosig    |          |          |
|          |          |          | natories |          |          |
+----------+----------+----------+----------+----------+----------+
| E        |          | Add and  | Value    | [NOT     |          |
| DTMTSG-8 |          | reduce   | does not | READ     |          |
|          |          | delete   | exceed   | Y]{.stat |          |
|          |          | users    | max      | us-macro |          |
|          |          |          | number   | .aui-    |          |
|          |          |          | of       | lozenge} |          |
|          |          |          | cosig    |          |          |
|          |          |          | natories |          |          |
+----------+----------+----------+----------+----------+----------+
| E        | Select   | Select   | Displays | [NOT     |          |
| DTMTSG-9 | cos      | main     | all      | READ     |          |
|          | ignatory | cos      | cosig    | Y]{.stat |          |
|          |          | ignatory | natories | us-macro |          |
|          |          | dropdown | a        | .aui-    |          |
|          |          |          | vailable | lozenge} |          |
|          |          |          | in the   |          |          |
|          |          |          | wallet   |          |          |
|          |          |          | except   |          |          |
|          |          |          | selected |          |          |
|          |          |          | cosigner |          |          |
|          |          |          | from     |          |          |
|          |          |          | other    |          |          |
|          |          |          | cos      |          |          |
|          |          |          | ignatory |          |          |
+----------+----------+----------+----------+----------+----------+
| ED       |          | Select   | Displays | [NOT     |          |
| TMTSG-10 |          | other    | all      | READ     |          |
|          |          | cos      | cosig    | Y]{.stat |          |
|          |          | ignatory | natories | us-macro |          |
|          |          | dropdown | a        | .aui-    |          |
|          |          |          | vailable | lozenge} |          |
|          |          |          | in the   |          |          |
|          |          |          | wallet   |          |          |
|          |          |          | except   |          |          |
|          |          |          | selected |          |          |
|          |          |          | cosigner |          |          |
|          |          |          | from     |          |          |
|          |          |          | main     |          |          |
|          |          |          | cos      |          |          |
|          |          |          | ignatory |          |          |
+----------+----------+----------+----------+----------+----------+
| ED       | Password | Leave    | Displays | [NOT     |          |
| TMTSG-11 |          | password | password | READ     |          |
|          |          | field    | is       | Y]{.stat |          |
|          |          | empty    | required | us-macro |          |
|          |          |          | error    | .aui-    |          |
|          |          |          |          | lozenge} |          |
+----------+----------+----------+----------+----------+----------+
| ED       | Clear    | Click    | Scheme,  | [NOT     |          |
| TMTSG-12 |          | clear    | added    | READ     |          |
|          |          |          | Cosi     | Y]{.stat |          |
|          |          |          | gnatory, | us-macro |          |
|          |          |          | removing | .aui-    |          |
|          |          |          | cos      | lozenge} |          |
|          |          |          | ignatory |          |          |
|          |          |          | and      |          |          |
|          |          |          | password |          |          |
|          |          |          | field    |          |          |
|          |          |          | are      |          |          |
|          |          |          | reset to |          |          |
|          |          |          | default  |          |          |
+----------+----------+----------+----------+----------+----------+
| ED       | Send     | Click    | Edit     | [NOT     |          |
| TMTSG-13 |          | send     | multisig | READ     |          |
|          |          | when     | account  | Y]{.stat |          |
|          |          | password |          | us-macro |          |
|          |          | field is |          | .aui-    |          |
|          |          | filled   |          | lozenge} |          |
+----------+----------+----------+----------+----------+----------+
| ED       |          | Click    | Send     | [NOT     |          |
| TMTSG-14 |          | send     | button   | READ     |          |
|          |          | when     | is       | Y]{.stat |          |
|          |          | scheme   | disabled | us-macro |          |
|          |          | values   |          | .aui-    |          |
|          |          | are      |          | lozenge} |          |
|          |          | adjusted |          |          |          |
|          |          | to 0     |          |          |          |
+----------+----------+----------+----------+----------+----------+
| ED       |          | Click    | Send     | [NOT     |          |
| TMTSG-15 |          | send     | button   | READ     |          |
|          |          | when any | is       | Y]{.stat |          |
|          |          | of the   | disabled | us-macro |          |
|          |          | above    |          | .aui-    |          |
|          |          | are not  |          | lozenge} |          |
|          |          | f        |          |          |          |
|          |          | ulfilled |          |          |          |
+----------+----------+----------+----------+----------+----------+
| ED       |          | Click    | Displays | [NOT     |          |
| TMTSG-16 |          | send     | password | READ     |          |
|          |          | when     | invalid  | Y]{.stat |          |
|          |          | password | error    | us-macro |          |
|          |          | is       |          | .aui-    |          |
|          |          | invalid  |          | lozenge} |          |
+----------+----------+----------+----------+----------+----------+
:::

::: table-wrap
+----------+----------+----------+----------+----------+----------+
| ## Serv  |          |          |          |          |          |
| ices {#T |          |          |          |          |          |
| estCases |          |          |          |          |          |
| -0.0.7-S |          |          |          |          |          |
| ervices} |          |          |          |          |          |
+----------+----------+----------+----------+----------+----------+
| ###      |          |          |          |          |          |
| Namespac |          |          |          |          |          |
| es {#Tes |          |          |          |          |          |
| tCases-0 |          |          |          |          |          |
| .0.7-Nam |          |          |          |          |          |
| espaces} |          |          |          |          |          |
+----------+----------+----------+----------+----------+----------+
| **Test   | **Test   | **Test   | **       | **       | **       |
| Case     | Sce      | steps**  | Expected | Status** | Remark** |
| ID**     | narios** |          | result** |          |          |
+----------+----------+----------+----------+----------+----------+
| NMSPC-1  | Register | Click on | Shows a  | [PAS     |          |
|          |          | the      | dropdown | S]{.stat |          |
|          |          | arrow    | list of  | us-macro |          |
|          |          | under    | a        | .aui     |          |
|          |          | "Na      | vailable | -lozenge |          |
|          |          | mespace" | options. | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | Goes to  | [PAS     |          |
|          |          | "R       | "Na      | S]{.stat |          |
|          |          | egister" | mespaces | us-macro |          |
|          |          |          | \>       | .aui     |          |
|          |          |          | Create"  | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | Shows a  | [PAS     |          |
|          |          | the      | dropdown | S]{.stat |          |
|          |          | address  | list of  | us-macro |          |
|          |          | under    | a        | .aui     |          |
|          |          | the      | vailable | -lozenge |          |
|          |          | account  | a        | .aui-    |          |
|          |          | name.    | ccounts. | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Select   | Shows    | [PAS     |          |
|          |          | an       | that the | S]{.stat |          |
|          |          | account. | specific | us-macro |          |
|          |          |          | account  | .aui     |          |
|          |          |          | is       | -lozenge |          |
|          |          |          | s        | .aui-    |          |
|          |          |          | elected. | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Enter    | No       | [PAS     |          |
|          |          | valid    | message  | S]{.stat |          |
|          |          | n        | is       | us-macro |          |
|          |          | amespace | shown.   | .aui     |          |
|          |          | name.    |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | Shows a  | [PAS     |          |
|          |          | "Select  | dropdown | S]{.stat |          |
|          |          | na       | list of  | us-macro |          |
|          |          | mespace" | a        | .aui     |          |
|          |          |          | vailable | -lozenge |          |
|          |          |          | nam      | .aui-    |          |
|          |          |          | espaces. | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Select   | Shows    | [PAS     |          |
|          |          | "New     | that     | S]{.stat |          |
|          |          | Root     | "New     | us-macro |          |
|          |          | Na       | Root     | .aui     |          |
|          |          | mespace" | Na       | -lozenge |          |
|          |          |          | mespace" | .aui-    |          |
|          |          |          | is       | lozenge- |          |
|          |          |          | s        | success} |          |
|          |          |          | elected. |          |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Enter    | No       | [PAS     |          |
|          |          | valid    | message  | S]{.stat |          |
|          |          | rental   | is       | us-macro |          |
|          |          | duration | shown.   | .aui     |          |
|          |          | in the   |          | -lozenge |          |
|          |          | "D       |          | .aui-    |          |
|          |          | uration" |          | lozenge- |          |
|          |          | input    |          | success} |          |
|          |          | field.   |          |          |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Enter    | No       | [PAS     |          |
|          |          | valid    | message  | S]{.stat |          |
|          |          | wallet   | is       | us-macro |          |
|          |          | p        | shown.   | .aui     |          |
|          |          | assword. |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | N        | [PAS     |          |
|          |          | "        | amespace | S]{.stat |          |
|          |          | Create". | is       | us-macro |          |
|          |          |          | created  | .aui     |          |
|          |          |          | after    | -lozenge |          |
|          |          |          | the      | .aui-    |          |
|          |          |          | tra      | lozenge- |          |
|          |          |          | nsaction | success} |          |
|          |          |          | is       |          |          |
|          |          |          | co       |          |          |
|          |          |          | nfirmed. |          |          |
+----------+----------+----------+----------+----------+----------+
| NMPSC-2  | Extend   | Click on | Shows a  | [PAS     |          |
|          | Duration | the      | dropdown | S]{.stat |          |
|          |          | arrow    | list of  | us-macro |          |
|          |          | under    | a        | .aui     |          |
|          |          | "Na      | vailable | -lozenge |          |
|          |          | mespace" | options. | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | Goes to  | [PAS     |          |
|          |          | "Extend  | "Na      | S]{.stat |          |
|          |          | D        | mespaces | us-macro |          |
|          |          | uration" | \>       | .aui     |          |
|          |          |          | Extend"  | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | Shows a  | [PAS     |          |
|          |          | the      | dropdown | S]{.stat |          |
|          |          | address  | list of  | us-macro |          |
|          |          | under    | a        | .aui     |          |
|          |          | the      | vailable | -lozenge |          |
|          |          | account  | a        | .aui-    |          |
|          |          | name.    | ccounts. | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | Shows a  | [PAS     |          |
|          |          | "Select  | dropdown | S]{.stat |          |
|          |          | na       | list of  | us-macro |          |
|          |          | mespace" | a        | .aui     |          |
|          |          |          | vailable | -lozenge |          |
|          |          |          | nam      | .aui-    |          |
|          |          |          | espaces. | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Select   | Shows    | [PAS     |          |
|          |          | an       | the name | S]{.stat |          |
|          |          | existing | of the   | us-macro |          |
|          |          | n        | selected | .aui     |          |
|          |          | amespace | na       | -lozenge |          |
|          |          | in the   | mespace. | .aui-    |          |
|          |          | account. |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Enter    | No       | [PAS     |          |
|          |          | valid    | message  | S]{.stat |          |
|          |          | rental   | is       | us-macro |          |
|          |          | duration | shown.   | .aui     |          |
|          |          | in the   |          | -lozenge |          |
|          |          | "D       |          | .aui-    |          |
|          |          | uration" |          | lozenge- |          |
|          |          | input    |          | success} |          |
|          |          | field.   |          |          |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Enter    | No       | [PAS     |          |
|          |          | valid    | message  | S]{.stat |          |
|          |          | wallet   | is       | us-macro |          |
|          |          | p        | shown.   | .aui     |          |
|          |          | assword. |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | N        | [PAS     |          |
|          |          | "        | amespace | S]{.stat |          |
|          |          | Create". | is       | us-macro |          |
|          |          |          | created  | .aui     |          |
|          |          |          | after    | -lozenge |          |
|          |          |          | the      | .aui-    |          |
|          |          |          | tra      | lozenge- |          |
|          |          |          | nsaction | success} |          |
|          |          |          | is       |          |          |
|          |          |          | co       |          |          |
|          |          |          | nfirmed. |          |          |
+----------+----------+----------+----------+----------+----------+
| ###      |          |          |          |          |          |
| Assets { |          |          |          |          |          |
| #TestCas |          |          |          |          |          |
| es-0.0.7 |          |          |          |          |          |
| -Assets} |          |          |          |          |          |
+----------+----------+----------+----------+----------+----------+
| ASST-1   | Create   | Click on | Shows a  | [PAS     |          |
|          |          | the      | dropdown | S]{.stat |          |
|          |          | arrow    | list of  | us-macro |          |
|          |          | under    | a        | .aui     |          |
|          |          | "        | vailable | -lozenge |          |
|          |          | Assets". | options. | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | Goes to  | [PAS     |          |
|          |          | "        | "Assets  | S]{.stat |          |
|          |          | Create". | \>       | us-macro |          |
|          |          |          | Create"  | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Enter a  | No       | [PAS     |          |
|          |          | valid    | message  | S]{.stat |          |
|          |          | number   | is       | us-macro |          |
|          |          | in the   | shown.   | .aui     |          |
|          |          | "Divis   |          | -lozenge |          |
|          |          | ibility" |          | .aui-    |          |
|          |          | input    |          | lozenge- |          |
|          |          | field.   |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Enter a  | No       | [PAS     |          |
|          |          | valid    | message  | S]{.stat |          |
|          |          | number   | is       | us-macro |          |
|          |          | in the   | shown.   | .aui     |          |
|          |          | "Supply" |          | -lozenge |          |
|          |          | input    |          | .aui-    |          |
|          |          | field.   |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | Checkbox | [PAS     |          |
|          |          | the      | is       | S]{.stat |          |
|          |          | checkbox | ticked.  | us-macro |          |
|          |          | on       |          | .aui     |          |
|          |          | "Trans   |          | -lozenge |          |
|          |          | ferable" |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | Checkbox | [PAS     |          |
|          |          | the      | is       | S]{.stat |          |
|          |          | checkbox | ticked.  | us-macro |          |
|          |          | on       |          | .aui     |          |
|          |          | "Supply  |          | -lozenge |          |
|          |          | Mutable" |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Enter    | No       | [PAS     |          |
|          |          | valid    | message  | S]{.stat |          |
|          |          | wallet   | is       | us-macro |          |
|          |          | p        | shown.   | .aui     |          |
|          |          | assword. |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | Asset is | [PAS     |          |
|          |          | "        | created. | S]{.stat |          |
|          |          | Create". |          | us-macro |          |
|          |          |          |          | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| ASST-2   | Modify   | Click on | Shows a  | [PAS     |          |
|          | Supply   | the      | dropdown | S]{.stat |          |
|          |          | arrow    | list of  | us-macro |          |
|          |          | under    | a        | .aui     |          |
|          |          | "        | vailable | -lozenge |          |
|          |          | Assets". | options. | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | Goes to  | [PAS     |          |
|          |          | "Modify  | "Assets  | S]{.stat |          |
|          |          | Supply". | \>       | us-macro |          |
|          |          |          | Modify   | .aui     |          |
|          |          |          | Supply"  | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | A list   | [PAS     |          |
|          |          | "Select  | of       | S]{.stat |          |
|          |          | asset".  | a        | us-macro |          |
|          |          |          | vailable | .aui     |          |
|          |          |          | assets   | -lozenge |          |
|          |          |          | are      | .aui-    |          |
|          |          |          | shown.   | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Select   | Shows    | [PAS     |          |
|          |          | one of   | the      | S]{.stat |          |
|          |          | the      | asset    | us-macro |          |
|          |          | assets.  | s        | .aui     |          |
|          |          |          | elected. | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | Shows a  | [PAS     |          |
|          |          | "Inc     | list of  | S]{.stat |          |
|          |          | rease/De | "I       | us-macro |          |
|          |          | crease". | ncrease" | .aui     |          |
|          |          |          | and      | -lozenge |          |
|          |          |          | "De      | .aui-    |          |
|          |          |          | crease". | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Select   | Shows    | [PAS     |          |
|          |          | "In      | "I       | S]{.stat |          |
|          |          | crease". | ncrease" | us-macro |          |
|          |          |          | is       | .aui     |          |
|          |          |          | s        | -lozenge |          |
|          |          |          | elected. | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Enter a  | No       | [PAS     |          |
|          |          | valid    | message  | S]{.stat |          |
|          |          | number   | is       | us-macro |          |
|          |          | in the   | shown.   | .aui     |          |
|          |          | "        |          | -lozenge |          |
|          |          | Quantity |          | .aui-    |          |
|          |          | of       |          | lozenge- |          |
|          |          | In       |          | success} |          |
|          |          | crease/D |          |          |          |
|          |          | ecrease" |          |          |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Enter    | No       | [PAS     |          |
|          |          | valid    | message  | S]{.stat |          |
|          |          | wallet   | is       | us-macro |          |
|          |          | p        | shown.   | .aui     |          |
|          |          | assword. |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | Supply   | [PAS     |          |
|          |          | "        | has      | S]{.stat |          |
|          |          | Create". | i        | us-macro |          |
|          |          |          | ncreased | .aui     |          |
|          |          |          | by the   | -lozenge |          |
|          |          |          | entered  | .aui-    |          |
|          |          |          | amount.  | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| ### Mai  |          |          |          | [NOT     |          |
| nnet Swa |          |          |          | READ     |          |
| p {#Test |          |          |          | Y]{.stat |          |
| Cases-0. |          |          |          | us-macro |          |
| 0.7-Main |          |          |          | .aui-    |          |
| netSwap} |          |          |          | lozenge} |          |
+----------+----------+----------+----------+----------+----------+
|          |          |          |          |          |          |
+----------+----------+----------+----------+----------+----------+
| ### Add  |          |          |          |          |          |
| ress Boo |          |          |          |          |          |
| k {#Test |          |          |          |          |          |
| Cases-0. |          |          |          |          |          |
| 0.7-Addr |          |          |          |          |          |
| essBook} |          |          |          |          |          |
+----------+----------+----------+----------+----------+----------+
| ADRSBK-1 | Add      | Click on | Shows a  | [PAS     |          |
|          | Contact  | the      | dropdown | S]{.stat |          |
|          |          | arrow    | list of  | us-macro |          |
|          |          | under    | a        | .aui     |          |
|          |          | "Address | vailable | -lozenge |          |
|          |          | Book"    | options. | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | Goes to  | [PAS     |          |
|          |          | "Add     | "Address | S]{.stat |          |
|          |          | C        | Book \>  | us-macro |          |
|          |          | ontacts" | Add      | .aui     |          |
|          |          |          | C        | -lozenge |          |
|          |          |          | ontacts" | .aui-    |          |
|          |          |          | page.    | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Enter    | No       | [PAS     |          |
|          |          | contact  | message  | S]{.stat |          |
|          |          | name in  | is       | us-macro |          |
|          |          | the      | shown.   | .aui     |          |
|          |          | "Name"   |          | -lozenge |          |
|          |          | input    |          | .aui-    |          |
|          |          | field    |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Enter    | No       | [PAS     |          |
|          |          | valid    | message  | S]{.stat |          |
|          |          | address  | is       | us-macro |          |
|          |          | of the   | shown.   | .aui     |          |
|          |          | contact. |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | New      | [PAS     |          |
|          |          | "Save"   | contact  | S]{.stat |          |
|          |          |          | is       | us-macro |          |
|          |          |          | added.   | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| ADRSBK-2 | Edit     | Click on | Shows a  | [PAS     |          |
|          |          | the      | dropdown | S]{.stat |          |
|          |          | arrow    | list of  | us-macro |          |
|          |          | under    | a        | .aui     |          |
|          |          | "Address | vailable | -lozenge |          |
|          |          | Book"    | options. | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | Goes to  | [PAS     |          |
|          |          | "List"   | "Address | S]{.stat |          |
|          |          |          | Book \>  | us-macro |          |
|          |          |          | List"    | .aui     |          |
|          |          |          | page.    | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | An "Edit | [PAS     |          |
|          |          | the edit | this     | S]{.stat |          |
|          |          | icon     | contact" | us-macro |          |
|          |          | under on | pop-up   | .aui     |          |
|          |          | one of   | will be  | -lozenge |          |
|          |          | the      | shown.   | .aui-    |          |
|          |          | a        |          | lozenge- |          |
|          |          | vailable |          | success} |          |
|          |          | c        |          |          |          |
|          |          | ontacts. |          |          |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Change   | No       | [PAS     |          |
|          |          | the name | message  | S]{.stat |          |
|          |          | of the   | is       | us-macro |          |
|          |          | contact. | shown.   | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Change   | No       | [PAS     |          |
|          |          | the      | message  | S]{.stat |          |
|          |          | address  | is       | us-macro |          |
|          |          | to       | shown.   | .aui     |          |
|          |          | another  |          | -lozenge |          |
|          |          | valid    |          | .aui-    |          |
|          |          | address. |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | The new  | [PAS     |          |
|          |          | "Save"   | changes  | S]{.stat |          |
|          |          |          | are      | us-macro |          |
|          |          |          | r        | .aui     |          |
|          |          |          | eflected | -lozenge |          |
|          |          |          | on the   | .aui-    |          |
|          |          |          | list.    | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| ADRSBK-2 | Export   | Click on | Shows a  | [PAS     |          |
|          |          | the      | dropdown | S]{.stat |          |
|          |          | arrow    | list of  | us-macro |          |
|          |          | under    | a        | .aui     |          |
|          |          | "Address | vailable | -lozenge |          |
|          |          | Book".   | options. | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | Goes to  | [PAS     |          |
|          |          | "List".  | "Address | S]{.stat |          |
|          |          |          | Book \>  | us-macro |          |
|          |          |          | List"    | .aui     |          |
|          |          |          | page.    | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | A file   | [PAS     |          |
|          |          | "        | in the   | S]{.stat |          |
|          |          | Export". | form of  | us-macro |          |
|          |          |          | .csv     | .aui     |          |
|          |          |          | will be  | -lozenge |          |
|          |          |          | do       | .aui-    |          |
|          |          |          | wnloaded | lozenge- |          |
|          |          |          | to the   | success} |          |
|          |          |          | local    |          |          |
|          |          |          | machine. |          |          |
+----------+----------+----------+----------+----------+----------+
| ### Wa   |          |          |          |          |          |
| llets {# |          |          |          |          |          |
| TestCase |          |          |          |          |          |
| s-0.0.7- |          |          |          |          |          |
| Wallets} |          |          |          |          |          |
+----------+----------+----------+----------+----------+----------+
| WLTSVC-1 | Change   |          |          | [NOT     |          |
|          | Password |          |          | READ     |          |
|          |          |          |          | Y]{.stat |          |
|          |          |          |          | us-macro |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge} |          |
+----------+----------+----------+----------+----------+----------+
| WLTSVC-2 | Export   |          |          | [NOT     |          |
|          |          |          |          | READ     |          |
|          |          |          |          | Y]{.stat |          |
|          |          |          |          | us-macro |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge} |          |
+----------+----------+----------+----------+----------+----------+
| WLTSVC-3 | Delete   | Click on | Shows a  | [PAS     |          |
|          |          | the      | dropdown | S]{.stat |          |
|          |          | arrow    | list of  | us-macro |          |
|          |          | under    | a        | .aui     |          |
|          |          | "        | vailable | -lozenge |          |
|          |          | Wallets" | options. | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | Shows    | [PAS     |          |
|          |          | "Delete" | all the  | S]{.stat |          |
|          |          |          | a        | us-macro |          |
|          |          |          | vailable | .aui     |          |
|          |          |          | wallets. | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | Proceeds | [PAS     |          |
|          |          | the      | to       | S]{.stat |          |
|          |          | delete   | confi    | us-macro |          |
|          |          | icon on  | rmation. | .aui     |          |
|          |          | one of   |          | -lozenge |          |
|          |          | the      |          | .aui-    |          |
|          |          | wallets  |          | lozenge- |          |
|          |          | that are |          | success} |          |
|          |          | av       |          |          |          |
|          |          | ailable. |          |          |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | A waring | [PAS     |          |
|          |          | "Delete" | message  | S]{.stat |          |
|          |          |          | will be  | us-macro |          |
|          |          |          | shown.   | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | The      | [PAS     |          |
|          |          | the "I   | checkbox | S]{.stat |          |
|          |          | have     | is       | us-macro |          |
|          |          | read the | ticked.  | .aui     |          |
|          |          | war      |          | -lozenge |          |
|          |          | ning..." |          | .aui-    |          |
|          |          | checkbox |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | The      | [PAS     |          |
|          |          | "Delete  | wallet   | S]{.stat |          |
|          |          | Now".    | is       | us-macro |          |
|          |          |          | delete   | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| ##       |          |          |          | [NOT     |          |
| # Nodes  |          |          |          | READ     |          |
| {#TestCa |          |          |          | Y]{.stat |          |
| ses-0.0. |          |          |          | us-macro |          |
| 7-Nodes} |          |          |          | .aui-    |          |
|          |          |          |          | lozenge} |          |
+----------+----------+----------+----------+----------+----------+
|          |          |          |          |          |          |
+----------+----------+----------+----------+----------+----------+
| ### At   |          |          |          | [NOT     |          |
| testatio |          |          |          | READ     |          |
| n {#Test |          |          |          | Y]{.stat |          |
| Cases-0. |          |          |          | us-macro |          |
| 0.7-Atte |          |          |          | .aui-    |          |
| station} |          |          |          | lozenge} |          |
+----------+----------+----------+----------+----------+----------+
|          |          |          |          |          |          |
+----------+----------+----------+----------+----------+----------+
| ##       |          |          |          | [NOT     |          |
| # Notifi |          |          |          | READ     |          |
| cations  |          |          |          | Y]{.stat |          |
| {#TestCa |          |          |          | us-macro |          |
| ses-0.0. |          |          |          | .aui-    |          |
| 7-Notifi |          |          |          | lozenge} |          |
| cations} |          |          |          |          |          |
+----------+----------+----------+----------+----------+----------+
|          |          |          |          |          |          |
+----------+----------+----------+----------+----------+----------+
| ###      |          |          |          | [NOT     |          |
| Voting { |          |          |          | READ     |          |
| #TestCas |          |          |          | Y]{.stat |          |
| es-0.0.7 |          |          |          | us-macro |          |
| -Voting} |          |          |          | .aui-    |          |
|          |          |          |          | lozenge} |          |
+----------+----------+----------+----------+----------+----------+
|          |          |          |          |          |          |
+----------+----------+----------+----------+----------+----------+
| ### St   |          |          |          | [NOT     |          |
| orage {# |          |          |          | READ     |          |
| TestCase |          |          |          | Y]{.stat |          |
| s-0.0.7- |          |          |          | us-macro |          |
| Storage} |          |          |          | .aui-    |          |
|          |          |          |          | lozenge} |          |
+----------+----------+----------+----------+----------+----------+
|          |          |          |          |          |          |
+----------+----------+----------+----------+----------+----------+
| ### S    |          |          |          | [NOT     |          |
| irius Gi |          |          |          | READ     |          |
| ft {#Tes |          |          |          | Y]{.stat |          |
| tCases-0 |          |          |          | us-macro |          |
| .0.7-Sir |          |          |          | .aui-    |          |
| iusGift} |          |          |          | lozenge} |          |
+----------+----------+----------+----------+----------+----------+
|          |          |          |          |          |          |
+----------+----------+----------+----------+----------+----------+
| #        |          |          |          | [NOT     |          |
| ## Aggre |          |          |          | READ     |          |
| gate Tra |          |          |          | Y]{.stat |          |
| nsaction |          |          |          | us-macro |          |
|  {#TestC |          |          |          | .aui-    |          |
| ases-0.0 |          |          |          | lozenge} |          |
| .7-Aggre |          |          |          |          |          |
| gateTran |          |          |          |          |          |
| saction} |          |          |          |          |          |
+----------+----------+----------+----------+----------+----------+
| ####     |          |          |          |          |          |
|  Aggrega |          |          |          |          |          |
| te Compl |          |          |          |          |          |
| ete {#Te |          |          |          |          |          |
| stCases- |          |          |          |          |          |
| 0.0.7-Ag |          |          |          |          |          |
| gregateC |          |          |          |          |          |
| omplete} |          |          |          |          |          |
+----------+----------+----------+----------+----------+----------+
| AGGTXN-1 | Create   | Select a | The      |          |          |
|          | Inner    | valid    | selected |          |          |
|          | Tra      | account  | Account  |          |          |
|          | nsaction | from the | name and |          |          |
|          |          | Account  | address  |          |          |
|          |          | dropdown | is       |          |          |
|          |          | bar.     | shown.   |          |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | The      |          |          |
|          |          | the      | Contacts |          |          |
|          |          | Contacts | dropdown |          |          |
|          |          | icon     | bar is   |          |          |
|          |          | beside   | shown.   |          |          |
|          |          | the      |          |          |          |
|          |          | "Re      |          |          |          |
|          |          | cipient" |          |          |          |
|          |          | input    |          |          |          |
|          |          | field.   |          |          |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Select a | The      |          | Will     |
|          |          | valid    | selected |          | show     |
|          |          | Contact  | Contact  |          | Invalid  |
|          |          | from the | name and |          | R        |
|          |          | Contact  | address  |          | ecipient |
|          |          | dropdown | is       |          | error    |
|          |          | bar.     | shown.   |          | message  |
|          |          |          |          |          | even if  |
|          |          |          |          |          | the      |
|          |          |          |          |          | address  |
|          |          |          |          |          | is       |
|          |          |          |          |          | valid.   |
+----------+----------+----------+----------+----------+----------+
|          |          | Enter a  | No error |          |          |
|          |          | valid    | message  |          |          |
|          |          | XPX      | is       |          |          |
|          |          | amount   | shown.   |          |          |
|          |          | in the   |          |          |          |
|          |          | "Send    |          |          |          |
|          |          | XPX"     |          |          |          |
|          |          | input    |          |          |          |
|          |          | field.   |          |          |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Enter a  | No error |          |          |
|          |          | valid    | message  |          |          |
|          |          | message  | is       |          |          |
|          |          | in the   | shown.   |          |          |
|          |          | "        |          |          |          |
|          |          | Message" |          |          |          |
|          |          | input    |          |          |          |
|          |          | field.   |          |          |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | Tra      |          |          |
|          |          | the      | nsaction |          |          |
|          |          | "Save"   | is saved |          |          |
|          |          | button.  | and      |          |          |
|          |          |          | shown in |          |          |
|          |          |          | the "My  |          |          |
|          |          |          | Tran     |          |          |
|          |          |          | saction" |          |          |
|          |          |          | column.  |          |          |
+----------+----------+----------+----------+----------+----------+
| AGGTXN-2 | Send     | Repeat   | Tran     |          |          |
|          | A        | the      | sactions |          |          |
|          | ggregate | steps in | is saved |          |          |
|          | Complete | AGGTXN-1 | and      |          |          |
|          | Tran     | to       | shown in |          |          |
|          | saction. | create   | the "My  |          |          |
|          |          | at least | Tran     |          |          |
|          |          | 3 Inner  | saction" |          |          |
|          |          | Tran     | column.  |          |          |
|          |          | sactions |          |          |          |
|          |          | with the |          |          |          |
|          |          | same     |          |          |          |
|          |          | Sender's |          |          |          |
|          |          | Account. |          |          |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Enter    | No error |          |          |
|          |          | valid    | message  |          |          |
|          |          | wallet   | is       |          |          |
|          |          | password | shown.   |          |          |
|          |          | in the   |          |          |          |
|          |          | "P       |          |          |          |
|          |          | assword" |          |          |          |
|          |          | input    |          |          |          |
|          |          | field.   |          |          |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | Tran     |          |          |
|          |          | the      | sactions |          |          |
|          |          | "Send    | are      |          |          |
|          |          | Ag       | succ     |          |          |
|          |          | gregate" | essfully |          |          |
|          |          | button.  | sent.    |          |          |
+----------+----------+----------+----------+----------+----------+
| AGGTXN-3 | Clear    | Select a | The      |          |          |
|          |          | valid    | selected |          |          |
|          |          | account  | Account  |          |          |
|          |          | from the | name and |          |          |
|          |          | Account  | address  |          |          |
|          |          | dropdown | is       |          |          |
|          |          | bar.     | shown.   |          |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | The      |          |          |
|          |          | the      | Contacts |          |          |
|          |          | Contacts | dropdown |          |          |
|          |          | icon     | bar is   |          |          |
|          |          | beside   | shown.   |          |          |
|          |          | the      |          |          |          |
|          |          | R        |          |          |          |
|          |          | ecipient |          |          |          |
|          |          | input    |          |          |          |
|          |          | field.   |          |          |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Select a | The      |          |          |
|          |          | valid    | selected |          |          |
|          |          | contact  | Contact  |          |          |
|          |          | from the | name and |          |          |
|          |          | contact  | address  |          |          |
|          |          | dropdown | is       |          |          |
|          |          | bar.     | shown.   |          |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Enter a  | No error |          |          |
|          |          | valid    | message  |          |          |
|          |          | XPX      | is       |          |          |
|          |          | amount   | shown.   |          |          |
|          |          | in the   |          |          |          |
|          |          | "Send    |          |          |          |
|          |          | XPX"     |          |          |          |
|          |          | input    |          |          |          |
|          |          | field.   |          |          |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Enter a  | No error |          |          |
|          |          | valid    | message  |          |          |
|          |          | message  | is       |          |          |
|          |          | in the   | shown.   |          |          |
|          |          | "        |          |          |          |
|          |          | Message" |          |          |          |
|          |          | input    |          |          |          |
|          |          | field.   |          |          |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Click on | All      |          |          |
|          |          | the      | inputs   |          |          |
|          |          | "Clear"  | are      |          |          |
|          |          | button.  | cleared. |          |          |
+----------+----------+----------+----------+----------+----------+
| AGGTXN-4 | XPX      | Enter a  | Shows    |          |          |
|          | Amount   | invalid  | "Insu    |          |          |
|          |          | XPX      | fficient |          |          |
|          |          | amount   | Balance" |          |          |
|          |          | in the   | error    |          |          |
|          |          | "Send    | message. |          |          |
|          |          | XPX"     |          |          |          |
|          |          | input    |          |          |          |
|          |          | field.   |          |          |          |
+----------+----------+----------+----------+----------+----------+
|          |          | Enter    | Shows    |          |          |
|          |          | letters  | "0".     |          |          |
|          |          | /symbols |          |          |          |
|          |          | in the   |          |          |          |
|          |          | "Send    |          |          |          |
|          |          | XPX"     |          |          |          |
|          |          | input    |          |          |          |
|          |          | field.   |          |          |          |
+----------+----------+----------+----------+----------+----------+
| AGGTXN-5 | Password | Enter a  | Shows    |          |          |
|          |          | invalid  | "Please  |          |          |
|          |          | password | enter    |          |          |
|          |          | in the   | wallet   |          |          |
|          |          | "P       | \[N      |          |          |
|          |          | assword" | ame\]\'s |          |          |
|          |          | input    | p        |          |          |
|          |          | field.   | assword" |          |          |
|          |          |          | error    |          |          |
|          |          |          | message. |          |          |
+----------+----------+----------+----------+----------+----------+
:::
:::

::: {.pageSection .group}
::: pageSectionHeader
## Attachments: {#attachments .pageSectionTitle}
:::

::: {.greybox align="left"}
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2366963817/2366963830)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[b6Y7vdCjGYj4Iz0F_WS65i2cmIOlSUT86qa6i_8b-nI5nMCdfPd8pzyZ7F00oJUCaExJm6trTRKlkKGVJ7Sk77IHaRM8J3xiPRDc7QBvZKdGSgTdYDf5PENJN1AGkDy16cx3ElRHYzDKpmmMJA](attachments/2366963817/2366963833)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[-bO8lWnCxvS5X986IxWgckBxaJCAbxhYl3-TF3royi6Q4j9TP6fotHOWiQ-il3_ryQNouMJ4csO5ZSgD_ZjKbkejc_edkj4PbVtm6f83nPyVS5LMbxvR1CSNaPwQrwZqw6pPpu1WRhThCx6m3A](attachments/2366963817/2366963836)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[JuJFRQviEuNr-LFhKKtzgok1mpF5HDikOIL1_xWg6aGr2qkQ8QSbxpffBmBBZjHP0mp8bWeQOwXRWRwlDCdz6gs25qus8boYnGvW4GVGSyi0cdVFcdwMCJyRp_oVci2AbNXYamEotatFLomrkg](attachments/2366963817/2366963839)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[image-20210910-065242.png](attachments/2366963817/2375876729.png)
(image/png)\
:::
:::
:::
:::

::: {#footer role="contentinfo"}
::: {.section .footer-body}
Document generated by Confluence on Nov 02, 2022 14:19

::: {#footer-logo}
[Atlassian](http://www.atlassian.com/)
:::
:::
:::
:::
