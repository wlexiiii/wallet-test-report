::: {#page}
::: {#main .aui-page-panel}
::: {#main-header}
::: {#breadcrumb-section}
1.  [ProximaX Tools](index.html)
2.  [Test Reports](Test-Reports_2443871313.html)
:::

# [ ProximaX Tools : Test Report - 1.1.8 -1 ]{#title-text} {#title-heading .pagetitle}
:::

::: {#content .view}
::: page-metadata
Created by [ davidwunarsa]{.author} on Jun 21, 2022
:::

::: {#main-content .wiki-content .group}
Date: 10/06/2022 - 10/06/2022\
Version: 1.1.8-1\
Test Environment: Mozilla Firefox (Version 100.0(64-bit)), Linux Ubuntu
20.04 LTS, Core i7-8750H CPU \@2.20GHz, 8GB RAM\
Staging Link: [ProximaX Web Wallet
(bsctestnetwallet)](https://bctestnetwallet.xpxsirius.io/#/){.external-link
rel="nofollow"}\
Browser: Mozilla Firefox (Version 100.0(64-bit))\
Testnet: Testnet 2

Reviewer:

-   [[Shin
    Neng](https://nemspfs.atlassian.net/wiki/people/5b84fef69170df2b44b5ef67?ref=confluence){.confluence-userlink
    .user-mention username="5b84fef69170df2b44b5ef67"
    account-id="5b84fef69170df2b44b5ef67" target="_blank"
    linked-resource-id="86540290" linked-resource-version="1"
    linked-resource-type="userinfo"
    base-url="https://nemspfs.atlassian.net/wiki"}\
    ]{.placeholder-inline-tasks}

::: {.toc-macro .rbtoc1667370001522}
-   [Main Page](#TestReport-1.1.8-1-MainPage)
    -   [Sign In](#TestReport-1.1.8-1-SignIn)
    -   [Create New Wallet](#TestReport-1.1.8-1-CreateNewWallet)
    -   [Create New Wallet From Private
        Key](#TestReport-1.1.8-1-CreateNewWalletFromPrivateKey)
    -   [Import wallet from .wlt file (Create Wallet from a Wallet
        Backup)](#TestReport-1.1.8-1-Importwalletfrom.wltfile(CreateWalletfromaWalletBackup))
-   [Dashboard](#TestReport-1.1.8-1-Dashboard)
-   [Side Menu Bar (Home
    Page)](#TestReport-1.1.8-1-SideMenuBar(HomePage))
-   [Transfer (New Design)](#TestReport-1.1.8-1-Transfer(NewDesign))
-   [Accounts](#TestReport-1.1.8-1-Accounts)
    -   [Select Creation Type](#TestReport-1.1.8-1-SelectCreationType)
        -   [Create a New Account in the same
            Wallet](#TestReport-1.1.8-1-CreateaNewAccountinthesameWallet)
        -   [Create a New Account from Private Key in the same
            Wallet](#TestReport-1.1.8-1-CreateaNewAccountfromPrivateKeyinthesameWallet)
    -   [Edit an existing
        Account](#TestReport-1.1.8-1-EditanexistingAccount)
        -   [Details](#TestReport-1.1.8-1-Details)
    -   [Convert to Multisig](#TestReport-1.1.8-1-ConverttoMultisig)
    -   [Edit Multisig](#TestReport-1.1.8-1-EditMultisig)
    -   [Outgoing Swap](#TestReport-1.1.8-1-OutgoingSwap)
-   [Services](#TestReport-1.1.8-1-Services)
    -   [Namespaces](#TestReport-1.1.8-1-Namespaces)
        -   [Register](#TestReport-1.1.8-1-Register)
        -   [Extend Duration](#TestReport-1.1.8-1-ExtendDuration)
    -   [Assets](#TestReport-1.1.8-1-Assets)
        -   [Create](#TestReport-1.1.8-1-Create)
        -   [Modify Supply](#TestReport-1.1.8-1-ModifySupply)
        -   [Link to Namespaces](#TestReport-1.1.8-1-LinktoNamespaces)
    -   [Swap](#TestReport-1.1.8-1-Swap)
        -   [NIS1](#TestReport-1.1.8-1-NIS1)
        -   [ETH](#TestReport-1.1.8-1-ETH)
        -   [BSC](#TestReport-1.1.8-1-BSC)
    -   [Address Book](#TestReport-1.1.8-1-AddressBook)
        -   [List](#TestReport-1.1.8-1-List)
        -   [Add Contacts](#TestReport-1.1.8-1-AddContacts)
    -   [Wallets](#TestReport-1.1.8-1-Wallets)
        -   [Change Password](#TestReport-1.1.8-1-ChangePassword)
        -   [Export](#TestReport-1.1.8-1-Export)
        -   [Delete](#TestReport-1.1.8-1-Delete)
    -   [Voting](#TestReport-1.1.8-1-Voting)
        -   [Create Poll](#TestReport-1.1.8-1-CreatePoll)
        -   [Vote](#TestReport-1.1.8-1-Vote)
        -   [View Results](#TestReport-1.1.8-1-ViewResults)
    -   [Storage](#TestReport-1.1.8-1-Storage)
        -   [Files](#TestReport-1.1.8-1-Files)
        -   [Upload File](#TestReport-1.1.8-1-UploadFile)
        -   [Send/Share](#TestReport-1.1.8-1-Send/Share)
    -   [Sirius Gift](#TestReport-1.1.8-1-SiriusGift)
        -   [Create](#TestReport-1.1.8-1-Create.1)
        -   [Redeem](#TestReport-1.1.8-1-Redeem)
    -   [Aggregate
        Transactions](#TestReport-1.1.8-1-AggregateTransactions)
        -   [Complete](#TestReport-1.1.8-1-Complete)
        -   [Bonded](#TestReport-1.1.8-1-Bonded)
:::

::: {.confluence-information-macro .confluence-information-macro-information}
[]{.aui-icon .aui-icon-small .aui-iconfont-info
.confluence-information-macro-icon}

::: confluence-information-macro-body
Status: [NOT READY]{.status-macro .aui-lozenge} [READY]{.status-macro
.aui-lozenge .aui-lozenge-current} [PASS]{.status-macro .aui-lozenge
.aui-lozenge-success} [FAIL]{.status-macro .aui-lozenge
.aui-lozenge-error} \| [YES]{.status-macro .aui-lozenge
.aui-lozenge-success} [NO]{.status-macro .aui-lozenge
.aui-lozenge-error}
:::
:::

::: table-wrap
+---------+---------+---------+---------+---------+---------+---------+
| #       |         |         |         |         |         |         |
| # Main  |         |         |         |         |         |         |
| Page {# |         |         |         |         |         |         |
| TestRep |         |         |         |         |         |         |
| ort-1.1 |         |         |         |         |         |         |
| .8-1-Ma |         |         |         |         |         |         |
| inPage} |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| **Test  | **Test  | **Test  | **E     | **S     | **R     | **Auto  |
| Case    | Scen    | steps** | xpected | tatus** | emark** | mated** |
| ID**    | arios** |         | r       |         |         |         |
|         |         |         | esult** |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| Main-1  | Sign in | Select  | Unable  | [PASS]  |         | [YES]   |
|         |         | wallet  | to sign | {.statu |         | {.statu |
|         |         | and     | in,     | s-macro |         | s-macro |
|         |         | click   | "Sign   | .aui-   |         | .aui-   |
|         |         | on      | In"     | lozenge |         | lozenge |
|         |         | "Sign   | button  | .aui-lo |         | .aui-lo |
|         |         | in"     | is      | zenge-s |         | zenge-s |
|         |         | button  | d       | uccess} |         | uccess} |
|         |         | without | isabled |         |         |         |
|         |         | e       | and     |         |         |         |
|         |         | ntering | error   |         |         |         |
|         |         | p       | message |         |         |         |
|         |         | assword | "P      |         |         |         |
|         |         |         | assword |         |         |         |
|         |         |         | is      |         |         |         |
|         |         |         | re      |         |         |         |
|         |         |         | quired" |         |         |         |
|         |         |         | is      |         |         |         |
|         |         |         | di      |         |         |         |
|         |         |         | splayed |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| Main-2  | Sign in | Select  | Go to   | [PASS]  |         | [YES]   |
|         |         | wallet, | the     | {.statu |         | {.statu |
|         |         | enter   | main    | s-macro |         | s-macro |
|         |         | p       | home    | .aui-   |         | .aui-   |
|         |         | assword | page of | lozenge |         | lozenge |
|         |         | and     | Sirius  | .aui-lo |         | .aui-lo |
|         |         | click   | Wallet  | zenge-s |         | zenge-s |
|         |         | on      |         | uccess} |         | uccess} |
|         |         | "Sign   |         |         |         |         |
|         |         | in"     |         |         |         |         |
|         |         | button  |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| Main-3  | Sign in | Enter   | Show an | [PASS]  |         | [YES]   |
|         |         | invalid | error   | {.statu |         | {.statu |
|         |         | p       | message | s-macro |         | s-macro |
|         |         | assword | "       | .aui-   |         | .aui-   |
|         |         |         | Invalid | lozenge |         | lozenge |
|         |         |         | Pa      | .aui-lo |         | .aui-lo |
|         |         |         | ssword" | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| Main-4  | Create  | Click   | Go to   | [PASS]  |         | [YES]   |
|         | New     | on      | screen  | {.statu |         | {.statu |
|         | Account | "Create | "Create | s-macro |         | s-macro |
|         | Wallet  | Account | Wallet" | .aui-   |         | .aui-   |
|         |         | Wallet" | with 3  | lozenge |         | lozenge |
|         |         | button  | se      | .aui-lo |         | .aui-lo |
|         |         |         | lection | zenge-s |         | zenge-s |
|         |         |         | types   | uccess} |         | uccess} |
|         |         |         | (new    |         |         |         |
|         |         |         | wallet, |         |         |         |
|         |         |         | private |         |         |         |
|         |         |         | key,    |         |         |         |
|         |         |         | wallet  |         |         |         |
|         |         |         | backup" |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ### S   |         |         |         |         |         |         |
| ign In  |         |         |         |         |         |         |
| {#TestR |         |         |         |         |         |         |
| eport-1 |         |         |         |         |         |         |
| .1.8-1- |         |         |         |         |         |         |
| SignIn} |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| S       | P       | Leave   | Show    | [PASS]  |         | [YES]   |
| IGNIN-1 | assword | the     | r       | {.statu |         | {.statu |
|         |         | field   | equired | s-macro |         | s-macro |
|         |         | empty   | field   | .aui-   |         | .aui-   |
|         |         |         | message | lozenge |         | lozenge |
|         |         |         | "P      | .aui-lo |         | .aui-lo |
|         |         |         | assword | zenge-s |         | zenge-s |
|         |         |         | is      | uccess} |         | uccess} |
|         |         |         | re      |         |         |         |
|         |         |         | quired" |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| S       |         | Place   | Show    | [FAIL]  | It      | [YES]   |
| IGNIN-2 |         | less    | message | {.statu | shows   | {.statu |
|         |         | than    | of      | s-macro | "p      | s-macro |
|         |         | r       | minimum | .aui-   | assword | .aui-   |
|         |         | equired | number  | lozenge | is      | lozenge |
|         |         | values  | of      | .aui-   | re      | .aui-lo |
|         |         |         | cha     | lozenge | quired" | zenge-s |
|         |         |         | racters | -error} | instead | uccess} |
|         |         |         | to      |         |         |         |
|         |         |         | enter   |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| S       |         | Enter   | Show an | [PASS]  |         | [YES]   |
| IGNIN-3 |         | invalid | error   | {.statu |         | {.statu |
|         |         | p       | message | s-macro |         | s-macro |
|         |         | assword | "       | .aui-   |         | .aui-   |
|         |         |         | Invalid | lozenge |         | lozenge |
|         |         |         | Pa      | .aui-lo |         | .aui-lo |
|         |         |         | ssword" | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| S       | After   | Click   | Enter   | [PASS]  |         | [YES]   |
| IGNIN-4 | se      | o       | the     | {.statu |         | {.statu |
|         | lecting | n "Sign | appl    | s-macro |         | s-macro |
|         | wallet  | in"     | ication | .aui-   |         | .aui-   |
|         | and     | button  | (main   | lozenge |         | lozenge |
|         | e       |         | home    | .aui-lo |         | .aui-lo |
|         | ntering |         | page of | zenge-s |         | zenge-s |
|         | p       |         | Sirius  | uccess} |         | uccess} |
|         | assword |         | Wallet) |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| S       | Sign    | Click   | Go back | [PASS]  |         | [YES]   |
| IGNIN-5 | Out     | on      | to Sign | {.statu |         | {.statu |
|         |         | "Sign   | In page | s-macro |         | s-macro |
|         |         | Out"    |         | .aui-   |         | .aui-   |
|         |         | button  |         | lozenge |         | lozenge |
|         |         |         |         | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| ###     |         |         |         |         |         |         |
|  Create |         |         |         |         |         |         |
|  New Wa |         |         |         |         |         |         |
| llet {# |         |         |         |         |         |         |
| TestRep |         |         |         |         |         |         |
| ort-1.1 |         |         |         |         |         |         |
| .8-1-Cr |         |         |         |         |         |         |
| eateNew |         |         |         |         |         |         |
| Wallet} |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| N       | Create\ | Click   | Go to   | [PASS]  |         | [YES]   |
| EWWLT-1 | (New    | on      | screen  | {.statu |         | {.statu |
|         | Wallet) | Create  | "Create | s-macro |         | s-macro |
|         |         | "New    | Wallet  | .aui-   |         | .aui-   |
|         |         | Wallet" | "       | lozenge |         | lozenge |
|         |         | button  |         | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| N       | Wallet  | Leave   | Show a  | [PASS]  |         | [YES]   |
| EWWLT-2 | name    | the     | message | {.statu |         | {.statu |
|         |         | field   | "Enter  | s-macro |         | s-macro |
|         |         | empty   | Wallet  | .aui-   |         | .aui-   |
|         |         |         | Name"   | lozenge |         | lozenge |
|         |         |         |         | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| N       |         | Set     | N/A     | [PASS]  |         | [YES]   |
| EWWLT-3 |         | special |         | {.statu |         | {.statu |
|         |         | cha     |         | s-macro |         | s-macro |
|         |         | racters |         | .aui-   |         | .aui-   |
|         |         |         |         | lozenge |         | lozenge |
|         |         |         |         | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| N       | Pa      | Leave   | Show an | [PASS]  |         | [YES]   |
| EWWLT-4 | ssword  | the     | error   | {.statu |         | {.statu |
|         |         | field   | message | s-macro |         | s-macro |
|         |         | empty   |         | .aui-   |         | .aui-   |
|         |         |         |         | lozenge |         | lozenge |
|         |         |         |         | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| N       |         | Set an  | Show a  | [PASS]  |         | [YES]   |
| EWWLT-5 |         | invalid | message | {.statu |         | {.statu |
|         |         | p       | "min    | s-macro |         | s-macro |
|         |         | assword | length  | .aui-   |         | .aui-   |
|         |         |         | 8"      | lozenge |         | lozenge |
|         |         |         |         | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| N       |         | Set     | special | [PASS]  |         | [YES]   |
| EWWLT-6 |         | special | cha     | {.statu |         | {.statu |
|         |         | cha     | racters | s-macro |         | s-macro |
|         |         | racters | can be  | .aui-   |         | .aui-   |
|         |         |         | used    | lozenge |         | lozenge |
|         |         |         | for     | .aui-lo |         | .aui-lo |
|         |         |         | p       | zenge-s |         | zenge-s |
|         |         |         | assword | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| N       |         | Place   | Show    | [PASS]  |         | [YES]   |
| EWWLT-7 |         | less    | message | {.statu |         | {.statu |
|         |         | than    | of      | s-macro |         | s-macro |
|         |         | r       | minimum | .aui-   |         | .aui-   |
|         |         | equired | number  | lozenge |         | lozenge |
|         |         | values  | of      | .aui-lo |         | .aui-lo |
|         |         |         | cha     | zenge-s |         | zenge-s |
|         |         |         | racters | uccess} |         | uccess} |
|         |         |         | to      |         |         |         |
|         |         |         | enter\  |         |         |         |
|         |         |         | "min    |         |         |         |
|         |         |         | length  |         |         |         |
|         |         |         | 8"      |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| N       | Confirm | Leave   | Show a  | [PASS]  |         | [YES]   |
| EWWLT-8 | p       | the     | m       | {.statu |         | {.statu |
|         | assword | field   | essage\ | s-macro |         | s-macro |
|         |         | empty   | "P      | .aui-   |         | .aui-   |
|         |         |         | assword | lozenge |         | lozenge |
|         |         |         | doesn't | .aui-lo |         | .aui-lo |
|         |         |         | match"  | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| N       |         | Enter a | Show a  | [PASS]  |         | [YES]   |
| EWWLT-9 |         | di      | m       | {.statu |         | {.statu |
|         |         | fferent | essage\ | s-macro |         | s-macro |
|         |         | p       | "P      | .aui-   |         | .aui-   |
|         |         | assword | assword | lozenge |         | lozenge |
|         |         |         | doesn't | .aui-lo |         | .aui-lo |
|         |         |         | match"  | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Set     | special | [PASS]  |         | [YES]   |
| WWLT-10 |         | special | cha     | {.statu |         | {.statu |
|         |         | cha     | racters | s-macro |         | s-macro |
|         |         | racters | can be  | .aui-   |         | .aui-   |
|         |         |         | used    | lozenge |         | lozenge |
|         |         |         | for     | .aui-lo |         | .aui-lo |
|         |         |         | p       | zenge-s |         | zenge-s |
|         |         |         | assword | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Place   | Show a  | [PASS]  |         | [YES]   |
| WWLT-11 |         | less or | m       | {.statu |         | {.statu |
|         |         | more    | essage\ | s-macro |         | s-macro |
|         |         | than    | "P      | .aui-   |         | .aui-   |
|         |         | r       | assword | lozenge |         | lozenge |
|         |         | equired | doesn't | .aui-lo |         | .aui-lo |
|         |         | values  | match"  | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| NE      | Eye     | Click   | Show /  | [PASS]  |         | [YES]   |
| WWLT-12 | Icons   | on      | hide    | {.statu |         | {.statu |
|         |         | "Pa     | the     | s-macro |         | s-macro |
|         |         | ssword" | p       | .aui-   |         | .aui-   |
|         |         | eye     | assword | lozenge |         | lozenge |
|         |         | icon    |         | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Click   | Show /  | [PASS]  |         | [YES]   |
| WWLT-13 |         | on      | hide    | {.statu |         | {.statu |
|         |         | "       | the     | s-macro |         | s-macro |
|         |         | Confirm | p       | .aui-   |         | .aui-   |
|         |         | pa      | assword | lozenge |         | lozenge |
|         |         | ssword" |         | .aui-lo |         | .aui-lo |
|         |         | eye     |         | zenge-s |         | zenge-s |
|         |         | icon    |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| NE      | Create  | Click   | Send a  | [PASS]  |         | [YES]   |
| WWLT-14 |         | on      | confi   | {.statu |         | {.statu |
|         |         | "Create | rmation | s-macro |         | s-macro |
|         |         | Wallet" | message | .aui-   |         | .aui-   |
|         |         | button  | and     | lozenge |         | lozenge |
|         |         |         | create  | .aui-lo |         | .aui-lo |
|         |         |         | the     | zenge-s |         | zenge-s |
|         |         |         | wallet  | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| ### Cr  |         |         |         |         |         |         |
| eate Ne |         |         |         |         |         |         |
| w Walle |         |         |         |         |         |         |
| t From  |         |         |         |         |         |         |
| Private |         |         |         |         |         |         |
|  Key {# |         |         |         |         |         |         |
| TestRep |         |         |         |         |         |         |
| ort-1.1 |         |         |         |         |         |         |
| .8-1-Cr |         |         |         |         |         |         |
| eateNew |         |         |         |         |         |         |
| WalletF |         |         |         |         |         |         |
| romPriv |         |         |         |         |         |         |
| ateKey} |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      | Create  | Click   | Go to   | [PASS]  |         | [YES]   |
| WWLT-15 | Wallet\ | on      | screen  | {.statu |         | {.statu |
|         | (From a | Create  | "Create | s-macro |         | s-macro |
|         | Private | Wallet  | Wallet  | .aui-   |         | .aui-   |
|         | Key)    | "From a | from a  | lozenge |         | lozenge |
|         |         | Private | Private | .aui-lo |         | .aui-lo |
|         |         | Key"    | Key"    | zenge-s |         | zenge-s |
|         |         | button  |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| NE      | Private | Leave   | Show an | [PASS]  |         | [YES]   |
| WWLT-16 | key     | the     | error   | {.statu |         | {.statu |
|         |         | field   | message | s-macro |         | s-macro |
|         |         | empty   | "       | .aui-   |         | .aui-   |
|         |         |         | Invalid | lozenge |         | lozenge |
|         |         |         | private | .aui-lo |         | .aui-lo |
|         |         |         | key"    | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Set an  | Show an | [PASS]  |         | [YES]   |
| WWLT-17 |         | invalid | error   | {.statu |         | {.statu |
|         |         | value   | message | s-macro |         | s-macro |
|         |         |         | "       | .aui-   |         | .aui-   |
|         |         |         | Invalid | lozenge |         | lozenge |
|         |         |         | private | .aui-lo |         | .aui-lo |
|         |         |         | key"    | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| NE      | Wallet  | Leave   | Show a  | [PASS]  |         | [YES]   |
| WWLT-18 | name    | the     | message | {.statu |         | {.statu |
|         |         | field   | "Enter  | s-macro |         | s-macro |
|         |         | empty   | Wallet  | .aui-   |         | .aui-   |
|         |         |         | Name"   | lozenge |         | lozenge |
|         |         |         |         | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Set     | N/A     | [PASS]  |         | [YES]   |
| WWLT-19 |         | special |         | {.statu |         | {.statu |
|         |         | cha     |         | s-macro |         | s-macro |
|         |         | racters |         | .aui-   |         | .aui-   |
|         |         |         |         | lozenge |         | lozenge |
|         |         |         |         | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| NE      | Pa      | Leave   | Show a  | [PASS]  |         | [YES]   |
| WWLT-20 | ssword  | the     | message | {.statu |         | {.statu |
|         |         | field   | "min    | s-macro |         | s-macro |
|         |         | empty   | length  | .aui-   |         | .aui-   |
|         |         |         | 8"      | lozenge |         | lozenge |
|         |         |         |         | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Set an  | Show a  | [PASS]  |         | [YES]   |
| WWLT-21 |         | invalid | message | {.statu |         | {.statu |
|         |         | p       | "min    | s-macro |         | s-macro |
|         |         | assword | length  | .aui-   |         | .aui-   |
|         |         |         | 8"      | lozenge |         | lozenge |
|         |         |         |         | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Set     | N/A     | [PASS]  |         | [YES]   |
| WWLT-22 |         | special |         | {.statu |         | {.statu |
|         |         | cha     |         | s-macro |         | s-macro |
|         |         | racters |         | .aui-   |         | .aui-   |
|         |         |         |         | lozenge |         | lozenge |
|         |         |         |         | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Place   | Show    | [PASS]  |         | [YES]   |
| WWLT-23 |         | less    | message | {.statu |         | {.statu |
|         |         | than    | of      | s-macro |         | s-macro |
|         |         | r       | minimum | .aui-   |         | .aui-   |
|         |         | equired | number  | lozenge |         | lozenge |
|         |         | values  | of      | .aui-lo |         | .aui-lo |
|         |         |         | cha     | zenge-s |         | zenge-s |
|         |         |         | racters | uccess} |         | uccess} |
|         |         |         | to      |         |         |         |
|         |         |         | enter\  |         |         |         |
|         |         |         | "min    |         |         |         |
|         |         |         | length  |         |         |         |
|         |         |         | 8"      |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      | Confirm | Leave   | Show a  | [PASS]  |         | [YES]   |
| WWLT-24 | p       | the     | message | {.statu |         | {.statu |
|         | assword | field   | "P      | s-macro |         | s-macro |
|         |         | empty   | assword | .aui-   |         | .aui-   |
|         |         |         | doesn't | lozenge |         | lozenge |
|         |         |         | match"  | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Enter a | Show a  | [PASS]  |         | [YES]   |
| WWLT-25 |         | di      | message | {.statu |         | {.statu |
|         |         | fferent | "P      | s-macro |         | s-macro |
|         |         | p       | assword | .aui-   |         | .aui-   |
|         |         | assword | doesn't | lozenge |         | lozenge |
|         |         |         | match"  | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Set     | N/A     | [PASS]  |         | [YES]   |
| WWLT-26 |         | special |         | {.statu |         | {.statu |
|         |         | cha     |         | s-macro |         | s-macro |
|         |         | racters |         | .aui-   |         | .aui-   |
|         |         |         |         | lozenge |         | lozenge |
|         |         |         |         | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
|         |         |         |         |         |         | -       |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Place   | Show a  | [PASS]  |         | [YES]   |
| WWLT-27 |         | less or | message | {.statu |         | {.statu |
|         |         | more    | "P      | s-macro |         | s-macro |
|         |         | than    | assword | .aui-   |         | .aui-   |
|         |         | r       | doesn't | lozenge |         | lozenge |
|         |         | equired | match"\ | .aui-lo |         | .aui-lo |
|         |         | values  |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| NE      | Eye     | Click   | Show /  | [PASS]  |         | [YES]   |
| WWLT-28 | icons   | on      | hide    | {.statu |         | {.statu |
|         |         | "       | the     | s-macro |         | s-macro |
|         |         | Private | private | .aui-   |         | .aui-   |
|         |         | key"    | key     | lozenge |         | lozenge |
|         |         | eye     |         | .aui-lo |         | .aui-lo |
|         |         | icon    |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Click   | Show /  | [PASS]  |         | [YES]   |
| WWLT-29 |         | on      | hide    | {.statu |         | {.statu |
|         |         | "Pa     | the     | s-macro |         | s-macro |
|         |         | ssword" | p       | .aui-   |         | .aui-   |
|         |         | eye     | assword | lozenge |         | lozenge |
|         |         | icon    |         | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Click   | Show /  | [PASS]  |         | [YES]   |
| WWLT-30 |         | on      | hide    | {.statu |         | {.statu |
|         |         | "       | the     | s-macro |         | s-macro |
|         |         | Confirm | p       | .aui-   |         | .aui-   |
|         |         | pa      | assword | lozenge |         | lozenge |
|         |         | ssword" |         | .aui-lo |         | .aui-lo |
|         |         | eye     |         | zenge-s |         | zenge-s |
|         |         | icon    |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| NE      | N/A     | Click   | Send a  | [PASS]  |         | [YES]   |
| WWLT-31 |         | on      | confi   | {.statu |         | {.statu |
|         |         | "       | rmation | s-macro |         | s-macro |
|         |         | Create" | message | .aui-   |         | .aui-   |
|         |         | button  | and     | lozenge |         | lozenge |
|         |         |         | create  | .aui-lo |         | .aui-lo |
|         |         |         | the     | zenge-s |         | zenge-s |
|         |         |         | wallet  | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| ### Imp |         |         |         |         |         |         |
| ort wal |         |         |         |         |         |         |
| let fro |         |         |         |         |         |         |
| m .wlt  |         |         |         |         |         |         |
| file (C |         |         |         |         |         |         |
| reate W |         |         |         |         |         |         |
| allet f |         |         |         |         |         |         |
| rom a W |         |         |         |         |         |         |
| allet B |         |         |         |         |         |         |
| ackup)  |         |         |         |         |         |         |
| {#TestR |         |         |         |         |         |         |
| eport-1 |         |         |         |         |         |         |
| .1.8-1- |         |         |         |         |         |         |
| Importw |         |         |         |         |         |         |
| alletfr |         |         |         |         |         |         |
| om.wltf |         |         |         |         |         |         |
| ile(Cre |         |         |         |         |         |         |
| ateWall |         |         |         |         |         |         |
| etfroma |         |         |         |         |         |         |
| WalletB |         |         |         |         |         |         |
| ackup)} |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      | Import\ | Click   | Go to   | [PASS]  |         | [YES]   |
| WWLT-32 | (From a | on      | screen  | {.statu |         | {.statu |
|         | Wallet  | "From a | "Create | s-macro |         | s-macro |
|         | Backup) | wallet  | Wallet  | .aui-   |         | .aui-   |
|         |         | backup" | from a  | lozenge |         | lozenge |
|         |         | button  | Wallet  | .aui-lo |         | .aui-lo |
|         |         |         | Backup" | zenge-s |         | zenge-s |
|         |         |         | and     | uccess} |         | uccess} |
|         |         |         | import  |         |         |         |
|         |         |         | button  |         |         |         |
|         |         |         | av      |         |         |         |
|         |         |         | ailable |         |         |         |
|         |         |         | to      |         |         |         |
|         |         |         | browse  |         |         |         |
|         |         |         | for the |         |         |         |
|         |         |         | .wlt    |         |         |         |
|         |         |         | file    |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Already | Go back | [PASS]  |         | [YES]   |
| WWLT-33 |         | have a  | to Sign | {.statu |         | {.statu |
|         |         | Sirius  | In page | s-macro |         | s-macro |
|         |         | Wallet  |         | .aui-   |         | .aui-   |
|         |         | a       |         | lozenge |         | lozenge |
|         |         | ccount, |         | .aui-lo |         | .aui-lo |
|         |         | click   |         | zenge-s |         | zenge-s |
|         |         | on      |         | uccess} |         | uccess} |
|         |         | "Sign   |         |         |         |         |
|         |         | in      |         |         |         |         |
|         |         | here"   |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
:::

::: table-wrap
+---------+---------+---------+---------+---------+---------+---------+
| ##      |         |         |         |         |         |         |
|  Dashbo |         |         |         |         |         |         |
| ard {#T |         |         |         |         |         |         |
| estRepo |         |         |         |         |         |         |
| rt-1.1. |         |         |         |         |         |         |
| 8-1-Das |         |         |         |         |         |         |
| hboard} |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| **Test  | **Test  | **Test  | **E     | **S     | **R     | **Auto  |
| Case    | Scen    | steps** | xpected | tatus** | emark** | mated** |
| ID**    | arios** |         | r       |         |         |         |
|         |         |         | esult** |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-1  | Home    | Click   | Back to | [PASS]  |         | [YES]   |
|         |         | "Home"  | da      | {.statu |         | {.statu |
|         |         | icon    | shboard | s-macro |         | s-macro |
|         |         |         | home    | .aui-   |         | .aui-   |
|         |         |         | page    | lozenge |         | lozenge |
|         |         |         |         | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-2  | +New    | Click   | Users   | [PASS]  |         | [YES]   |
|         |         | "+New"  | can     | {.statu |         | {.statu |
|         |         | button  | select  | s-macro |         | s-macro |
|         |         |         | to      | .aui-   |         | .aui-   |
|         |         |         | t       | lozenge |         | lozenge |
|         |         |         | ransfer | .aui-lo |         | .aui-lo |
|         |         |         | xpx,    | zenge-s |         | zenge-s |
|         |         |         | create  | uccess} |         | uccess} |
|         |         |         | digital |         |         |         |
|         |         |         | asset,  |         |         |         |
|         |         |         | na      |         |         |         |
|         |         |         | mespace |         |         |         |
|         |         |         | and     |         |         |         |
|         |         |         | account |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-3  |         | After   | User    | [PASS]  |         | [YES]   |
|         |         | c       | d       | {.statu |         | {.statu |
|         |         | licking | irected | s-macro |         | s-macro |
|         |         | new     | to      | .aui-   |         | .aui-   |
|         |         | button, | create  | lozenge |         | lozenge |
|         |         | click   | asset   | .aui-lo |         | .aui-lo |
|         |         | digital | page    | zenge-s |         | zenge-s |
|         |         | asset   |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-4  |         | After   | User    | [PASS]  |         | [YES]   |
|         |         | c       | d       | {.statu |         | {.statu |
|         |         | licking | irected | s-macro |         | s-macro |
|         |         | new     | to      | .aui-   |         | .aui-   |
|         |         | button, | create  | lozenge |         | lozenge |
|         |         | click   | na      | .aui-lo |         | .aui-lo |
|         |         | na      | mespace | zenge-s |         | zenge-s |
|         |         | mespace | page    | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-5  |         | After   | User    | [PASS]  |         | [YES]   |
|         |         | c       | d       | {.statu |         | {.statu |
|         |         | licking | irected | s-macro |         | s-macro |
|         |         | new     | to      | .aui-   |         | .aui-   |
|         |         | button, | create  | lozenge |         | lozenge |
|         |         | click   | account | .aui-lo |         | .aui-lo |
|         |         | account | page    | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
|         |         | After   | User    | [PASS]  |         | [YES]   |
|         |         | c       | d       | {.statu |         | {.statu |
|         |         | licking | irected | s-macro |         | s-macro |
|         |         | new     | to      | .aui-   |         | .aui-   |
|         |         | button, | t       | lozenge |         | lozenge |
|         |         | click   | ransfer | .aui-lo |         | .aui-lo |
|         |         | t       | xpx     | zenge-s |         | zenge-s |
|         |         | ransfer | page    | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-6  | Beg     | Click   | A list  | [PASS]  |         | [YES]   |
|         | inner's | on      | of      | {.statu |         | {.statu |
|         | guide   | q       | b       | s-macro |         | s-macro |
|         |         | uestion | eginner | .aui-   |         | .aui-   |
|         |         | mark    | guides  | lozenge |         | lozenge |
|         |         | button  | av      | .aui-lo |         | .aui-lo |
|         |         |         | ailable | zenge-s |         | zenge-s |
|         |         |         | for     | uccess} |         | uccess} |
|         |         |         | user    |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-7  | Notif   | Click   | User    | [PASS]  |         | [YES]   |
|         | ication | on      | d       | {.statu |         | {.statu |
|         |         | notif   | irected | s-macro |         | s-macro |
|         |         | ication | to      | .aui-   |         | .aui-   |
|         |         | button  | notif   | lozenge |         | lozenge |
|         |         |         | ication | .aui-lo |         | .aui-lo |
|         |         |         | page    | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-8  | S       | Click   | User    | [PASS]  |         | [YES]   |
|         | ettings | on      | d       | {.statu |         | {.statu |
|         |         | s       | irected | s-macro |         | s-macro |
|         |         | ettings | to      | .aui-   |         | .aui-   |
|         |         | button  | s       | lozenge |         | lozenge |
|         |         |         | ettings | .aui-lo |         | .aui-lo |
|         |         |         | page    | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-9  | O       | Click   | An      | [FAIL]  | [       |         |
|         | verview | on      | o       | {.statu | [[]{.a  |         |
|         |         | "Ov     | verview | s-macro | ui-icon |         |
|         |         | erview" | of      | .aui-   | .aui-ic |         |
|         |         | tab     | user's  | lozenge | on-wait |         |
|         |         |         | assets, | .aui-   | .issue  |         |
|         |         |         | nam     | lozenge | -placeh |         |
|         |         |         | espaces | -error} | older}W |         |
|         |         |         | and     |         | LT-38]( |         |
|         |         |         | recent  |         | https:/ |         |
|         |         |         | trans   |         | /nemspf |         |
|         |         |         | actions |         | s.atlas |         |
|         |         |         |         |         | sian.ne |         |
|         |         |         |         |         | t/brows |         |
|         |         |         |         |         | e/WLT-3 |         |
|         |         |         |         |         | 8){.jir |         |
|         |         |         |         |         | a-issue |         |
|         |         |         |         |         | -key} - |         |
|         |         |         |         |         | [       |         |
|         |         |         |         |         | Getting |         |
|         |         |         |         |         | issue   |         |
|         |         |         |         |         | d       |         |
|         |         |         |         |         | etails\ |         |
|         |         |         |         |         | ...]{.s |         |
|         |         |         |         |         | ummary} |         |
|         |         |         |         |         | [STATUS |         |
|         |         |         |         |         | ]{.aui- |         |
|         |         |         |         |         | lozenge |         |
|         |         |         |         |         | .aui-   |         |
|         |         |         |         |         | lozenge |         |
|         |         |         |         |         | -subtle |         |
|         |         |         |         |         | .aui-l  |         |
|         |         |         |         |         | ozenge- |         |
|         |         |         |         |         | default |         |
|         |         |         |         |         | .issu   |         |
|         |         |         |         |         | e-place |         |
|         |         |         |         |         | holder} |         |
|         |         |         |         |         | ]{      |         |
|         |         |         |         |         | .conflu |         |
|         |         |         |         |         | ence-ji |         |
|         |         |         |         |         | m-macro |         |
|         |         |         |         |         | .jir    |         |
|         |         |         |         |         | a-issue |         |
|         |         |         |         |         | jir     |         |
|         |         |         |         |         | a-key=" |         |
|         |         |         |         |         | WLT-38" |         |
|         |         |         |         |         | c       |         |
|         |         |         |         |         | lient-i |         |
|         |         |         |         |         | d="SING |         |
|         |         |         |         |         | LE_5581 |         |
|         |         |         |         |         | e30e-87 |         |
|         |         |         |         |         | 6a-3bbe |         |
|         |         |         |         |         | -9902-8 |         |
|         |         |         |         |         | 6eb613c |         |
|         |         |         |         |         | b022_24 |         |
|         |         |         |         |         | 9924812 |         |
|         |         |         |         |         | 9_5b142 |         |
|         |         |         |         |         | d79091e |         |
|         |         |         |         |         | 9f17116 |         |
|         |         |         |         |         | 363a5"} |         |
|         |         |         |         |         | [       |         |
|         |         |         |         |         | [[]{.a  |         |
|         |         |         |         |         | ui-icon |         |
|         |         |         |         |         | .aui-ic |         |
|         |         |         |         |         | on-wait |         |
|         |         |         |         |         | .issue  |         |
|         |         |         |         |         | -placeh |         |
|         |         |         |         |         | older}W |         |
|         |         |         |         |         | LT-39]( |         |
|         |         |         |         |         | https:/ |         |
|         |         |         |         |         | /nemspf |         |
|         |         |         |         |         | s.atlas |         |
|         |         |         |         |         | sian.ne |         |
|         |         |         |         |         | t/brows |         |
|         |         |         |         |         | e/WLT-3 |         |
|         |         |         |         |         | 9){.jir |         |
|         |         |         |         |         | a-issue |         |
|         |         |         |         |         | -key} - |         |
|         |         |         |         |         | [       |         |
|         |         |         |         |         | Getting |         |
|         |         |         |         |         | issue   |         |
|         |         |         |         |         | d       |         |
|         |         |         |         |         | etails\ |         |
|         |         |         |         |         | ...]{.s |         |
|         |         |         |         |         | ummary} |         |
|         |         |         |         |         | [STATUS |         |
|         |         |         |         |         | ]{.aui- |         |
|         |         |         |         |         | lozenge |         |
|         |         |         |         |         | .aui-   |         |
|         |         |         |         |         | lozenge |         |
|         |         |         |         |         | -subtle |         |
|         |         |         |         |         | .aui-l  |         |
|         |         |         |         |         | ozenge- |         |
|         |         |         |         |         | default |         |
|         |         |         |         |         | .issu   |         |
|         |         |         |         |         | e-place |         |
|         |         |         |         |         | holder} |         |
|         |         |         |         |         | ]{      |         |
|         |         |         |         |         | .conflu |         |
|         |         |         |         |         | ence-ji |         |
|         |         |         |         |         | m-macro |         |
|         |         |         |         |         | .jir    |         |
|         |         |         |         |         | a-issue |         |
|         |         |         |         |         | jir     |         |
|         |         |         |         |         | a-key=" |         |
|         |         |         |         |         | WLT-39" |         |
|         |         |         |         |         | c       |         |
|         |         |         |         |         | lient-i |         |
|         |         |         |         |         | d="SING |         |
|         |         |         |         |         | LE_5581 |         |
|         |         |         |         |         | e30e-87 |         |
|         |         |         |         |         | 6a-3bbe |         |
|         |         |         |         |         | -9902-8 |         |
|         |         |         |         |         | 6eb613c |         |
|         |         |         |         |         | b022_24 |         |
|         |         |         |         |         | 9924812 |         |
|         |         |         |         |         | 9_5b142 |         |
|         |         |         |         |         | d79091e |         |
|         |         |         |         |         | 9f17116 |         |
|         |         |         |         |         | 363a5"} |         |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-10 | Assets  | Click   | D       | [PASS]  |         | [YES]   |
|         |         | on      | isplays | {.statu |         | {.statu |
|         |         | "       | a list  | s-macro |         | s-macro |
|         |         | Assets" | of      | .aui-   |         | .aui-   |
|         |         | tab     | user's  | lozenge |         | lozenge |
|         |         |         | assets  | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-11 | Nam     | Click   | D       | [PASS]  |         | [YES]   |
|         | espaces | on      | isplays | {.statu |         | {.statu |
|         |         | "Name   | a list  | s-macro |         | s-macro |
|         |         | spaces" | of      | .aui-   |         | .aui-   |
|         |         | tab     | user's  | lozenge |         | lozenge |
|         |         |         | nam     | .aui-lo |         | .aui-lo |
|         |         |         | espaces | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-12 | All     | Click   | D       | [PASS]  |         | [YES]   |
|         | Trans   | on "All | isplays | {.statu |         | {.statu |
|         | actions | transa  | a list  | s-macro |         | s-macro |
|         |         | ctions" | of      | .aui-   |         | .aui-   |
|         |         | tab     | user's  | lozenge |         | lozenge |
|         |         |         | trans   | .aui-lo |         | .aui-lo |
|         |         |         | actions | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-13 | Header  | Click   | Wallet  | [PASS]  |         | [YES]   |
|         | com     | on copy | address | {.statu |         | {.statu |
|         | ponents | wallet  | is      | s-macro |         | s-macro |
|         |         | address | copied  | .aui-   |         | .aui-   |
|         |         | button  | and a   | lozenge |         | lozenge |
|         |         |         | notif   | .aui-lo |         | .aui-lo |
|         |         |         | ication | zenge-s |         | zenge-s |
|         |         |         | is      | uccess} |         | uccess} |
|         |         |         | shown   |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-14 |         | Click   | User    | [PASS]  |         | [YES]   |
|         |         | on      | d       | {.statu |         | {.statu |
|         |         | "Swap"  | irected | s-macro |         | s-macro |
|         |         | button  | to swap | .aui-   |         | .aui-   |
|         |         |         | page    | lozenge |         | lozenge |
|         |         |         |         | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-15 |         | Click   | Display | [PASS]  |         | [YES]   |
|         |         | on      | QR Code | {.statu |         | {.statu |
|         |         | "Scan   | of      | s-macro |         | s-macro |
|         |         | QR      | wallet  | .aui-   |         | .aui-   |
|         |         | Code"   | address | lozenge |         | lozenge |
|         |         | button  |         | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-16 |         | Click   | User    | [PASS]  |         | [YES]   |
|         |         | on      | d       | {.statu |         | {.statu |
|         |         | "       | irected | s-macro |         | s-macro |
|         |         | Convert | to      | .aui-   |         | .aui-   |
|         |         | to      | m       | lozenge |         | lozenge |
|         |         | Mu      | ultisig | .aui-lo |         | .aui-lo |
|         |         | ltisig" | page    | zenge-s |         | zenge-s |
|         |         | button  |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-17 |         | Click   | User is | [PASS]  |         | [YES]   |
|         |         | on      | d       | {.statu |         | {.statu |
|         |         | "T      | irected | s-macro |         | s-macro |
|         |         | ransfer | to      | .aui-   |         | .aui-   |
|         |         | XPX"    | t       | lozenge |         | lozenge |
|         |         | button  | ransfer | .aui-lo |         | .aui-lo |
|         |         |         | xpx     | zenge-s |         | zenge-s |
|         |         |         | page    | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
:::

::: table-wrap
+---------+---------+---------+---------+---------+---------+---------+
| ##      |         |         |         |         |         |         |
|  Side M |         |         |         |         |         |         |
| enu Bar |         |         |         |         |         |         |
|  (Home  |         |         |         |         |         |         |
| Page) { |         |         |         |         |         |         |
| #TestRe |         |         |         |         |         |         |
| port-1. |         |         |         |         |         |         |
| 1.8-1-S |         |         |         |         |         |         |
| ideMenu |         |         |         |         |         |         |
| Bar(Hom |         |         |         |         |         |         |
| ePage)} |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| **Test  | **Test  | **Test  | **E     | **S     | **R     | **Auto  |
| Case    | Scen    | steps** | xpected | tatus** | emark** | mated** |
| ID**    | arios** |         | r       |         |         |         |
|         |         |         | esult** |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-1  | Account | Click   | User is | [PASS]  |         | [YES]   |
|         |         | on any  | d       | {.statu |         | {.statu |
|         |         | account | irected | s-macro |         | s-macro |
|         |         | under   | to the  | .aui-   |         | .aui-   |
|         |         | "Ac     | res     | lozenge |         | lozenge |
|         |         | counts" | pective | .aui-lo |         | .aui-lo |
|         |         |         | account | zenge-s |         | zenge-s |
|         |         |         | details | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-2  | Create  | Click   | User is | [PASS]  |         | [YES]   |
|         | New     | on      | d       | {.statu |         | {.statu |
|         | Account | "       | irected | s-macro |         | s-macro |
|         |         | +Create | to      | .aui-   |         | .aui-   |
|         |         | New     | "Create | lozenge |         | lozenge |
|         |         | A       | New     | .aui-lo |         | .aui-lo |
|         |         | ccount" | A       | zenge-s |         | zenge-s |
|         |         | under   | ccount" | uccess} |         | uccess} |
|         |         | "       | Page    |         |         |         |
|         |         | Default |         |         |         |         |
|         |         | A       |         |         |         |         |
|         |         | ccount" |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-3  | Na      | Click   | User is | [PASS]  |         | [YES]   |
|         | mespace | on      | d       | {.statu |         | {.statu |
|         |         | "Nam    | irected | s-macro |         | s-macro |
|         |         | espace" | to a    | .aui-   |         | .aui-   |
|         |         | under   | page to | lozenge |         | lozenge |
|         |         | "Quick  | create  | .aui-lo |         | .aui-lo |
|         |         | Action" | na      | zenge-s |         | zenge-s |
|         |         |         | mespace | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-4  |         | Leave   | Show an | [FAIL]  | "r      |         |
|         |         | name    | error   | {.statu | egister |         |
|         |         | empty   | message | s-macro | nam     |         |
|         |         |         | saying  | .aui-   | espace" |         |
|         |         |         | it's a  | lozenge | button  |         |
|         |         |         | r       | .aui-   | is      |         |
|         |         |         | equired | lozenge | di      |         |
|         |         |         | field   | -error} | sabled, |         |
|         |         |         |         |         | but no  |         |
|         |         |         |         |         | error   |         |
|         |         |         |         |         | message |         |
|         |         |         |         |         | yet     |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-5  |         | Leave   | show an | [FAIL]  | "r      |         |
|         |         | na      | error   | {.statu | egister |         |
|         |         | mespace | message | s-macro | nam     |         |
|         |         | not     | saying  | .aui-   | espace" |         |
|         |         | s       | it's    | lozenge | button  |         |
|         |         | elected | r       | .aui-   | is      |         |
|         |         |         | equired | lozenge | di      |         |
|         |         |         | to be   | -error} | sabled, |         |
|         |         |         | s       |         | but no  |         |
|         |         |         | elected |         | error   |         |
|         |         |         |         |         | message |         |
|         |         |         |         |         | yet     |         |
|         |         |         |         |         |         |         |
|         |         |         |         |         | [       |         |
|         |         |         |         |         | [[]{.a  |         |
|         |         |         |         |         | ui-icon |         |
|         |         |         |         |         | .aui-ic |         |
|         |         |         |         |         | on-wait |         |
|         |         |         |         |         | .issue  |         |
|         |         |         |         |         | -placeh |         |
|         |         |         |         |         | older}W |         |
|         |         |         |         |         | LT-54]( |         |
|         |         |         |         |         | https:/ |         |
|         |         |         |         |         | /nemspf |         |
|         |         |         |         |         | s.atlas |         |
|         |         |         |         |         | sian.ne |         |
|         |         |         |         |         | t/brows |         |
|         |         |         |         |         | e/WLT-5 |         |
|         |         |         |         |         | 4){.jir |         |
|         |         |         |         |         | a-issue |         |
|         |         |         |         |         | -key} - |         |
|         |         |         |         |         | [       |         |
|         |         |         |         |         | Getting |         |
|         |         |         |         |         | issue   |         |
|         |         |         |         |         | d       |         |
|         |         |         |         |         | etails\ |         |
|         |         |         |         |         | ...]{.s |         |
|         |         |         |         |         | ummary} |         |
|         |         |         |         |         | [STATUS |         |
|         |         |         |         |         | ]{.aui- |         |
|         |         |         |         |         | lozenge |         |
|         |         |         |         |         | .aui-   |         |
|         |         |         |         |         | lozenge |         |
|         |         |         |         |         | -subtle |         |
|         |         |         |         |         | .aui-l  |         |
|         |         |         |         |         | ozenge- |         |
|         |         |         |         |         | default |         |
|         |         |         |         |         | .issu   |         |
|         |         |         |         |         | e-place |         |
|         |         |         |         |         | holder} |         |
|         |         |         |         |         | ]{      |         |
|         |         |         |         |         | .conflu |         |
|         |         |         |         |         | ence-ji |         |
|         |         |         |         |         | m-macro |         |
|         |         |         |         |         | .jir    |         |
|         |         |         |         |         | a-issue |         |
|         |         |         |         |         | jir     |         |
|         |         |         |         |         | a-key=" |         |
|         |         |         |         |         | WLT-54" |         |
|         |         |         |         |         | c       |         |
|         |         |         |         |         | lient-i |         |
|         |         |         |         |         | d="SING |         |
|         |         |         |         |         | LE_5581 |         |
|         |         |         |         |         | e30e-87 |         |
|         |         |         |         |         | 6a-3bbe |         |
|         |         |         |         |         | -9902-8 |         |
|         |         |         |         |         | 6eb613c |         |
|         |         |         |         |         | b022_24 |         |
|         |         |         |         |         | 9924812 |         |
|         |         |         |         |         | 9_5b142 |         |
|         |         |         |         |         | d79091e |         |
|         |         |         |         |         | 9f17116 |         |
|         |         |         |         |         | 363a5"} |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-6  |         | Enter   | Shows   | [PASS]  |         | [YES]   |
|         |         | invalid | an      | {.statu |         | {.statu |
|         |         | name    | error   | s-macro |         | s-macro |
|         |         | (one    | message | .aui-   |         | .aui-   |
|         |         | char)   | to      | lozenge |         | lozenge |
|         |         |         | enter   | .aui-lo |         | .aui-lo |
|         |         |         | valid   | zenge-s |         | zenge-s |
|         |         |         | name    | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-7  |         | Enter   | Na      | [PASS]  |         | [YES]   |
|         |         | valid   | mespace | {.statu |         | {.statu |
|         |         | name,\  | created | s-macro |         | s-macro |
|         |         | Enter   | with id | .aui-   |         | .aui-   |
|         |         | d       | and     | lozenge |         | lozenge |
|         |         | uration | exp     | .aui-lo |         | .aui-lo |
|         |         | of      | iration | zenge-s |         | zenge-s |
|         |         | days,\  | ti      | uccess} |         | uccess} |
|         |         | Enter   | mestamp |         |         |         |
|         |         | correct |         |         |         |         |
|         |         | p       |         |         |         |         |
|         |         | assword |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-8  |         | Enter   | User is | [PASS]  |         | [YES]   |
|         |         | valid   | d       | {.statu |         | {.statu |
|         |         | name,\  | irected | s-macro |         | s-macro |
|         |         | Enter   | back to | .aui-   |         | .aui-   |
|         |         | d       | na      | lozenge |         | lozenge |
|         |         | uration | mespace | .aui-lo |         | .aui-lo |
|         |         | of      | page    | zenge-s |         | zenge-s |
|         |         | days,\  |         | uccess} |         | uccess} |
|         |         | Enter   |         |         |         |         |
|         |         | correct |         |         |         |         |
|         |         | pas     |         |         |         |         |
|         |         | sword,\ |         |         |         |         |
|         |         | Click   |         |         |         |         |
|         |         | "       |         |         |         |         |
|         |         | Cancel" |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-9  |         | Enter   | Shows   | [PASS]  |         | [YES]   |
|         |         | valid   | an      | {.statu |         | {.statu |
|         |         | name,\  | error   | s-macro |         | s-macro |
|         |         | Enter   | saying  | .aui-   |         | .aui-   |
|         |         | d       | p       | lozenge |         | lozenge |
|         |         | uration | assword | .aui-lo |         | .aui-lo |
|         |         | of      | is      | zenge-s |         | zenge-s |
|         |         | days,\  | r       | uccess} |         | uccess} |
|         |         | Leave   | equired |         |         |         |
|         |         | p       | and     |         |         |         |
|         |         | assword | r       |         |         |         |
|         |         | empty   | egister |         |         |         |
|         |         |         | button  |         |         |         |
|         |         |         | is      |         |         |         |
|         |         |         | d       |         |         |         |
|         |         |         | isabled |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-10 |         | Enter   | Shows   | [PASS]  |         | [YES]   |
|         |         | wrong   | an      | {.statu |         | {.statu |
|         |         | wallet  | error   | s-macro |         | s-macro |
|         |         | p       | saying  | .aui-   |         | .aui-   |
|         |         | assword | wallet  | lozenge |         | lozenge |
|         |         |         | p       | .aui-lo |         | .aui-lo |
|         |         |         | assword | zenge-s |         | zenge-s |
|         |         |         | is      | uccess} |         | uccess} |
|         |         |         | in      |         |         |         |
|         |         |         | correct |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-11 | Asset   | Click   | User is | [PASS]  |         | [YES]   |
|         |         | on      | d       | {.statu |         | {.statu |
|         |         | "Asset" | irected | s-macro |         | s-macro |
|         |         | under   | to      | .aui-   |         | .aui-   |
|         |         | "Quick  | "       | lozenge |         | lozenge |
|         |         | Action" | Assets" | .aui-lo |         | .aui-lo |
|         |         |         | page    | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-12 |         | Click   | User is | [PASS]  |         | [YES]   |
|         |         | on      | d       | {.statu |         | {.statu |
|         |         | "       | irected | s-macro |         | s-macro |
|         |         | +Create | to      | .aui-   |         | .aui-   |
|         |         | New     | "Create | lozenge |         | lozenge |
|         |         | Asset"  | Asset"  | .aui-lo |         | .aui-lo |
|         |         |         | page    | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-13 |         | Leave   | Show an | [PASS]  |         | [YES]   |
|         |         | supply, | error   | {.statu |         | {.statu |
|         |         | divis   | to      | s-macro |         | s-macro |
|         |         | ibility | enter   | .aui-   |         | .aui-   |
|         |         | and     | wallet  | lozenge |         | lozenge |
|         |         | wallet  | p       | .aui-lo |         | .aui-lo |
|         |         | p       | assword | zenge-s |         | zenge-s |
|         |         | assword |         | uccess} |         | uccess} |
|         |         | empty   |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-14 |         | Enter   | Asset   | [PASS]  |         | [YES]   |
|         |         | amount  | is      | {.statu |         | {.statu |
|         |         | of      | created | s-macro |         | s-macro |
|         |         | s       | with    | .aui-   |         | .aui-   |
|         |         | upply,\ | its     | lozenge |         | lozenge |
|         |         | Enter   | res     | .aui-lo |         | .aui-lo |
|         |         | divisib | pective | zenge-s |         | zenge-s |
|         |         | ility,\ | id and  | uccess} |         | uccess} |
|         |         | Enter   | details |         |         |         |
|         |         | correct |         |         |         |         |
|         |         | wallet  |         |         |         |         |
|         |         | p       |         |         |         |         |
|         |         | assword |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-15 |         | Enter   | Show an | [FAIL]  | No      |         |
|         |         | amount  | error   | {.statu | notifi  |         |
|         |         | of      | saying  | s-macro | cation, |         |
|         |         | s       | wallet  | .aui-   | nothing |         |
|         |         | upply,\ | p       | lozenge | h       |         |
|         |         | Enter   | assword | .aui-   | appened |         |
|         |         | divisib | is      | lozenge | at all. |         |
|         |         | ility,\ | in      | -error} | [       |         |
|         |         | Enter   | correct |         | [[]{.a  |         |
|         |         | wrong   |         |         | ui-icon |         |
|         |         | wallet  |         |         | .aui-ic |         |
|         |         | p       |         |         | on-wait |         |
|         |         | assword |         |         | .issue  |         |
|         |         |         |         |         | -placeh |         |
|         |         |         |         |         | older}W |         |
|         |         |         |         |         | LT-48]( |         |
|         |         |         |         |         | https:/ |         |
|         |         |         |         |         | /nemspf |         |
|         |         |         |         |         | s.atlas |         |
|         |         |         |         |         | sian.ne |         |
|         |         |         |         |         | t/brows |         |
|         |         |         |         |         | e/WLT-4 |         |
|         |         |         |         |         | 8){.jir |         |
|         |         |         |         |         | a-issue |         |
|         |         |         |         |         | -key} - |         |
|         |         |         |         |         | [       |         |
|         |         |         |         |         | Getting |         |
|         |         |         |         |         | issue   |         |
|         |         |         |         |         | d       |         |
|         |         |         |         |         | etails\ |         |
|         |         |         |         |         | ...]{.s |         |
|         |         |         |         |         | ummary} |         |
|         |         |         |         |         | [STATUS |         |
|         |         |         |         |         | ]{.aui- |         |
|         |         |         |         |         | lozenge |         |
|         |         |         |         |         | .aui-   |         |
|         |         |         |         |         | lozenge |         |
|         |         |         |         |         | -subtle |         |
|         |         |         |         |         | .aui-l  |         |
|         |         |         |         |         | ozenge- |         |
|         |         |         |         |         | default |         |
|         |         |         |         |         | .issu   |         |
|         |         |         |         |         | e-place |         |
|         |         |         |         |         | holder} |         |
|         |         |         |         |         | ]{      |         |
|         |         |         |         |         | .conflu |         |
|         |         |         |         |         | ence-ji |         |
|         |         |         |         |         | m-macro |         |
|         |         |         |         |         | .jir    |         |
|         |         |         |         |         | a-issue |         |
|         |         |         |         |         | jir     |         |
|         |         |         |         |         | a-key=" |         |
|         |         |         |         |         | WLT-48" |         |
|         |         |         |         |         | c       |         |
|         |         |         |         |         | lient-i |         |
|         |         |         |         |         | d="SING |         |
|         |         |         |         |         | LE_5581 |         |
|         |         |         |         |         | e30e-87 |         |
|         |         |         |         |         | 6a-3bbe |         |
|         |         |         |         |         | -9902-8 |         |
|         |         |         |         |         | 6eb613c |         |
|         |         |         |         |         | b022_24 |         |
|         |         |         |         |         | 9924812 |         |
|         |         |         |         |         | 9_5b142 |         |
|         |         |         |         |         | d79091e |         |
|         |         |         |         |         | 9f17116 |         |
|         |         |         |         |         | 363a5"} |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-16 | Wallets | Click   | D       | [PASS]  |         | [YES]   |
|         |         | on      | isplays | {.statu |         | {.statu |
|         |         | "W      | a list  | s-macro |         | s-macro |
|         |         | allets" | of      | .aui-   |         | .aui-   |
|         |         | under   | wallets | lozenge |         | lozenge |
|         |         | "Na     | av      | .aui-lo |         | .aui-lo |
|         |         | vigate" | ailable | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-17 |         | Click   | D       | [PASS]  |         | [YES]   |
|         |         | on the  | isplays | {.statu |         | {.statu |
|         |         | trash   | the     | s-macro |         | s-macro |
|         |         | icon of | delete  | .aui-   |         | .aui-   |
|         |         | the     | confi   | lozenge |         | lozenge |
|         |         | wallet  | rmation | .aui-lo |         | .aui-lo |
|         |         | to      | pop-up  | zenge-s |         | zenge-s |
|         |         | delete  |         | uccess} |         | uccess} |
|         |         | it      |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-18 |         | Click   | Wallet  | [PASS]  |         | [YES]   |
|         |         | on      | succe   | {.statu |         | {.statu |
|         |         | delete  | ssfully | s-macro |         | s-macro |
|         |         | now     | removed | .aui-   |         | .aui-   |
|         |         | button  | and a   | lozenge |         | lozenge |
|         |         |         | notif   | .aui-lo |         | .aui-lo |
|         |         |         | ication | zenge-s |         | zenge-s |
|         |         |         | is      | uccess} |         | uccess} |
|         |         |         | shown   |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-19 | A       | Click   | D       | [PASS]  |         | [YES]   |
|         | ccounts | on      | isplays | {.statu |         | {.statu |
|         |         | "Ac     | an      | s-macro |         | s-macro |
|         |         | counts" | o       | .aui-   |         | .aui-   |
|         |         | under   | verview | lozenge |         | lozenge |
|         |         | "Na     | of the  | .aui-lo |         | .aui-lo |
|         |         | vigate" | user's  | zenge-s |         | zenge-s |
|         |         |         | a       | uccess} |         | uccess} |
|         |         |         | ccounts |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-20 |         | Click   | D       | [PASS]  |         | [YES]   |
|         |         | on "My  | isplays | {.statu |         | {.statu |
|         |         | Ac      | user's  | s-macro |         | s-macro |
|         |         | counts" | a       | .aui-   |         | .aui-   |
|         |         | tab     | ccounts | lozenge |         | lozenge |
|         |         |         |         | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-21 |         | Click   | D       | [PASS]  |         | [YES]   |
|         |         | on      | isplays | {.statu |         | {.statu |
|         |         | "M      | user's  | s-macro |         | s-macro |
|         |         | ultisig | m       | .aui-   |         | .aui-   |
|         |         | Ac      | ultisig | lozenge |         | lozenge |
|         |         | counts" | a       | .aui-lo |         | .aui-lo |
|         |         | tab     | ccounts | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-22 |         | Click   | D       | [PASS]  |         | [YES]   |
|         |         | on      | isplays | {.statu |         | {.statu |
|         |         | "Other  | user's  | s-macro |         | s-macro |
|         |         | Ac      | other   | .aui-   |         | .aui-   |
|         |         | counts" | a       | lozenge |         | lozenge |
|         |         | tab     | ccounts | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-23 | Address | Click   | D       | [PASS]  |         | [YES]   |
|         | Book    | on      | isplays | {.statu |         | {.statu |
|         |         | "       | user's  | s-macro |         | s-macro |
|         |         | Address | address | .aui-   |         | .aui-   |
|         |         | Book"   | book    | lozenge |         | lozenge |
|         |         | under   | list    | .aui-lo |         | .aui-lo |
|         |         | "Na     |         | zenge-s |         | zenge-s |
|         |         | vigate" |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-24 |         | Click   | User    | [PASS]  |         | [YES]   |
|         |         | on      | d       | {.statu |         | {.statu |
|         |         | "+Add   | irected | s-macro |         | s-macro |
|         |         | New     | to "Add | .aui-   |         | .aui-   |
|         |         | A       | New     | lozenge |         | lozenge |
|         |         | ddress" | C       | .aui-lo |         | .aui-lo |
|         |         |         | ontact" | zenge-s |         | zenge-s |
|         |         |         | page    | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-25 |         | Enter   | Shows a | [PASS]  |         | [YES]   |
|         |         | valid   | message | {.statu |         | {.statu |
|         |         | ad      | saying  | s-macro |         | s-macro |
|         |         | dress,\ | name is | .aui-   |         | .aui-   |
|         |         | Leave   | r       | lozenge |         | lozenge |
|         |         | name    | equired | .aui-lo |         | .aui-lo |
|         |         | empty   |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-26 |         | Enter   | Show an | [PASS]  |         | [YES]   |
|         |         | name,\  | error   | {.statu |         | {.statu |
|         |         | Enter   | (       | s-macro |         | s-macro |
|         |         | invalid | address | .aui-   |         | .aui-   |
|         |         | address | is      | lozenge |         | lozenge |
|         |         |         | re      | .aui-lo |         | .aui-lo |
|         |         |         | quired) | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-27 |         | Enter   | Shows a | [PASS]  |         | [YES]   |
|         |         | name,   | message | {.statu |         | {.statu |
|         |         | place   | saying  | s-macro |         | s-macro |
|         |         | less or | address | .aui-   |         | .aui-   |
|         |         | more    | is      | lozenge |         | lozenge |
|         |         | than    | r       | .aui-lo |         | .aui-lo |
|         |         | r       | equired | zenge-s |         | zenge-s |
|         |         | equired |         | uccess} |         | uccess} |
|         |         | value   |         |         |         |         |
|         |         | for     |         |         |         |         |
|         |         | address |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-28 |         | Enter   | Shows a | [PASS]  |         | [YES]   |
|         |         | an      | message | {.statu |         | {.statu |
|         |         | address | saying  | s-macro |         | s-macro |
|         |         | that    | the     | .aui-   |         | .aui-   |
|         |         | already | address | lozenge |         | lozenge |
|         |         | exists  | exists  | .aui-lo |         | .aui-lo |
|         |         | in the  | in the  | zenge-s |         | zenge-s |
|         |         | wallet  | wallet  | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-29 |         | Enter   | New     | [PASS]  |         | [YES]   |
|         |         | name,\  | address | {.statu |         | {.statu |
|         |         | Enter   | added   | s-macro |         | s-macro |
|         |         | valid   | and     | .aui-   |         | .aui-   |
|         |         | ad      | di      | lozenge |         | lozenge |
|         |         | dress,\ | splayed | .aui-lo |         | .aui-lo |
|         |         | Click   | under   | zenge-s |         | zenge-s |
|         |         | save    | address | uccess} |         | uccess} |
|         |         | address | book    |         |         |         |
|         |         |         | list    |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-30 | Custom  | Enter   | Enter   | [PASS]  |         | [YES]   |
|         |         | name,\  | custom  | {.statu |         | {.statu |
|         |         | Enter   | group   | s-macro |         | s-macro |
|         |         | valid   | name    | .aui-   |         | .aui-   |
|         |         | ad      | pop up  | lozenge |         | lozenge |
|         |         | dress,\ | is      | .aui-lo |         | .aui-lo |
|         |         | Choose  | shown   | zenge-s |         | zenge-s |
|         |         | custom  |         | uccess} |         | uccess} |
|         |         | group   |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-31 |         | Enter   | New     | [PASS]  |         | [YES]   |
|         |         | valid   | address | {.statu |         | {.statu |
|         |         | custom  | added   | s-macro |         | s-macro |
|         |         | group   | and     | .aui-   |         | .aui-   |
|         |         | name,   | di      | lozenge |         | lozenge |
|         |         | save    | splayed | .aui-lo |         | .aui-lo |
|         |         | address | under   | zenge-s |         | zenge-s |
|         |         |         | address | uccess} |         | uccess} |
|         |         |         | book    |         |         |         |
|         |         |         | list    |         |         |         |
|         |         |         | with    |         |         |         |
|         |         |         | the     |         |         |         |
|         |         |         | custom  |         |         |         |
|         |         |         | group   |         |         |         |
|         |         |         | name    |         |         |         |
|         |         |         | created |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-32 | Edit    | Click   | User    | [PASS]  |         | [YES]   |
|         | address | on edit | d       | {.statu |         | {.statu |
|         |         | address | irected | s-macro |         | s-macro |
|         |         |         | to edit | .aui-   |         | .aui-   |
|         |         |         | contact | lozenge |         | lozenge |
|         |         |         | page    | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-33 |         | Edit    | Show an | [PASS]  |         | [YES]   |
|         |         | name    | error   | {.statu |         | {.statu |
|         |         | field   |         | s-macro |         | s-macro |
|         |         | to be   |         | .aui-   |         | .aui-   |
|         |         | empty   |         | lozenge |         | lozenge |
|         |         |         |         | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-34 |         | Edit    | Show an | [PASS]  |         | [YES]   |
|         |         | address | error   | {.statu |         | {.statu |
|         |         | to be   |         | s-macro |         | s-macro |
|         |         | invalid |         | .aui-   |         | .aui-   |
|         |         |         |         | lozenge |         | lozenge |
|         |         |         |         | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-35 |         | Edit    | A       | [PASS]  |         | [YES]   |
|         |         | name    | notif   | {.statu |         | {.statu |
|         |         | (valid  | ication | s-macro |         | s-macro |
|         |         | input   | saying  | .aui-   |         | .aui-   |
|         |         | name)   | contact | lozenge |         | lozenge |
|         |         | and     | updated | .aui-lo |         | .aui-lo |
|         |         | address | suc     | zenge-s |         | zenge-s |
|         |         | (valid  | cessful | uccess} |         | uccess} |
|         |         | input   | is      |         |         |         |
|         |         | a       | shown   |         |         |         |
|         |         | ddress) |         |         |         |         |
|         |         | and     |         |         |         |         |
|         |         | save    |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-36 | Remove  | Click   | Prompts | [PASS]  |         | [YES]   |
|         | address | on      | for     | {.statu |         | {.statu |
|         |         | remove  | user    | s-macro |         | s-macro |
|         |         | address | confi   | .aui-   |         | .aui-   |
|         |         |         | rmation | lozenge |         | lozenge |
|         |         |         |         | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-37 |         | Click   | Contact | [PASS]  |         | [YES]   |
|         |         | remove  | is      | {.statu |         | {.statu |
|         |         | contact | removed | s-macro |         | s-macro |
|         |         |         | from    | .aui-   |         | .aui-   |
|         |         |         | address | lozenge |         | lozenge |
|         |         |         | book    | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-38 | Import  | Click   | Prompts | [PASS]  |         |         |
|         | Contact | on      | for     | {.statu |         |         |
|         |         | import  | user to | s-macro |         |         |
|         |         | tab,    | choose  | .aui-   |         |         |
|         |         | click   | file to | lozenge |         |         |
|         |         | import  | add     | .aui-lo |         |         |
|         |         | button  | contact | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-39 | Export  | Click   | Contact | [PASS]  |         |         |
|         | Contact | on      | is      | {.statu |         |         |
|         |         | export  | dow     | s-macro |         |         |
|         |         | tab,    | nloaded | .aui-   |         |         |
|         |         | click   | to      | lozenge |         |         |
|         |         | export  | user's  | .aui-lo |         |         |
|         |         | button  | local   | zenge-s |         |         |
|         |         |         | machine | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| Menu-40 | Sign    | Click   | Go back | [PASS]  |         | [YES]   |
|         | Out     | on      | to Sign | {.statu |         | {.statu |
|         |         | "Sign   | In page | s-macro |         | s-macro |
|         |         | Out"    |         | .aui-   |         | .aui-   |
|         |         | button  |         | lozenge |         | lozenge |
|         |         |         |         | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
:::

::: table-wrap
+---------+---------+---------+---------+---------+---------+---------+
| ##      |         |         |         |         |         |         |
| Transfe |         |         |         |         |         |         |
| r (New  |         |         |         |         |         |         |
| Design) |         |         |         |         |         |         |
|  {#Test |         |         |         |         |         |         |
| Report- |         |         |         |         |         |         |
| 1.1.8-1 |         |         |         |         |         |         |
| -Transf |         |         |         |         |         |         |
| er(NewD |         |         |         |         |         |         |
| esign)} |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| **Test  | **Test  | **Test  | **E     | **S     | **R     | **Auto  |
| Case    | Scen    | steps** | xpected | tatus** | emark** | mated** |
| ID**    | arios** |         | r       |         |         |         |
|         |         |         | esult** |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-1  | Sender  | Click   | A drop  | [PASS]  |         | [YES]   |
|         | account | t       | down    | {.statu |         | {.statu |
|         | (T      | ransfer | list of | s-macro |         | s-macro |
|         | ransfer | from    | a       | .aui-   |         | .aui-   |
|         | from)   | account | ccounts | lozenge |         | lozenge |
|         |         |         | av      | .aui-lo |         | .aui-lo |
|         |         |         | ailable | zenge-s |         | zenge-s |
|         |         |         | in      | uccess} |         | uccess} |
|         |         |         | wallet  |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-2  |         | Select  | Sender  | [PASS]  |         | [YES]   |
|         |         | another | account | {.statu |         | {.statu |
|         |         | account | is      | s-macro |         | s-macro |
|         |         | from    | changed | .aui-   |         | .aui-   |
|         |         | drop    |         | lozenge |         | lozenge |
|         |         | down    |         | .aui-lo |         | .aui-lo |
|         |         | list    |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-3  | R       | Enter   | Icon    | [PASS]  |         | [YES]   |
|         | eceiver | invalid | saying  | {.statu |         | {.statu |
|         | account | wallet  | invalid | s-macro |         | s-macro |
|         | (T      | address |         | .aui-   |         | .aui-   |
|         | ransfer |         |         | lozenge |         | lozenge |
|         | to)     |         |         | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-4  |         | Click   | A drop  | [PASS]  |         | [YES]   |
|         |         | select  | down    | {.statu |         | {.statu |
|         |         | contact | list of | s-macro |         | s-macro |
|         |         |         | c       | .aui-   |         | .aui-   |
|         |         |         | ontacts | lozenge |         | lozenge |
|         |         |         | from    | .aui-lo |         | .aui-lo |
|         |         |         | address | zenge-s |         | zenge-s |
|         |         |         | book    | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-5  | T       | Leave   | Could   | [PASS]  |         | [YES]   |
|         | ransfer | t       | not     | {.statu |         | {.statu |
|         | amount  | ransfer | proceed | s-macro |         | s-macro |
|         |         | amount  | and     | .aui-   |         | .aui-   |
|         |         | as 0    | t       | lozenge |         | lozenge |
|         |         |         | ransfer | .aui-lo |         | .aui-lo |
|         |         |         | button  | zenge-s |         | zenge-s |
|         |         |         | is      | uccess} |         | uccess} |
|         |         |         | d       |         |         |         |
|         |         |         | isabled |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-6  | Message | Enter   | Tran    | [PASS]  |         | [YES]   |
|         |         | random  | saction | {.statu |         | {.statu |
|         |         | m       | Fee     | s-macro |         | s-macro |
|         |         | essages | in      | .aui-   |         | .aui-   |
|         |         |         | creases | lozenge |         | lozenge |
|         |         |         | as      | .aui-lo |         | .aui-lo |
|         |         |         | message | zenge-s |         | zenge-s |
|         |         |         | size    | uccess} |         | uccess} |
|         |         |         | in      |         |         |         |
|         |         |         | creases |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-7  |         | Enter   | P       | [FAIL]  | T       |         |
|         |         | more    | revents | {.statu | ransfer |         |
|         |         | than    | input   | s-macro | failed, |         |
|         |         | maximum | upon    | .aui-   | but     |         |
|         |         | of      | r       | lozenge | user    |         |
|         |         | message | eaching | .aui-   | can     |         |
|         |         | limit   | maximum | lozenge | still   |         |
|         |         |         | message | -error} | input   |         |
|         |         |         | limit   |         | message |         |
|         |         |         |         |         | ex      |         |
|         |         |         |         |         | ceeding |         |
|         |         |         |         |         | the     |         |
|         |         |         |         |         | limit   |         |
|         |         |         |         |         |         |         |
|         |         |         |         |         | [       |         |
|         |         |         |         |         | [[]{.a  |         |
|         |         |         |         |         | ui-icon |         |
|         |         |         |         |         | .aui-ic |         |
|         |         |         |         |         | on-wait |         |
|         |         |         |         |         | .iss    |         |
|         |         |         |         |         | ue-plac |         |
|         |         |         |         |         | eholder |         |
|         |         |         |         |         | }WLT-1] |         |
|         |         |         |         |         | (https: |         |
|         |         |         |         |         | //nemsp |         |
|         |         |         |         |         | fs.atla |         |
|         |         |         |         |         | ssian.n |         |
|         |         |         |         |         | et/brow |         |
|         |         |         |         |         | se/WLT- |         |
|         |         |         |         |         | 1){.jir |         |
|         |         |         |         |         | a-issue |         |
|         |         |         |         |         | -key} - |         |
|         |         |         |         |         | [       |         |
|         |         |         |         |         | Getting |         |
|         |         |         |         |         | issue   |         |
|         |         |         |         |         | d       |         |
|         |         |         |         |         | etails\ |         |
|         |         |         |         |         | ...]{.s |         |
|         |         |         |         |         | ummary} |         |
|         |         |         |         |         | [STATUS |         |
|         |         |         |         |         | ]{.aui- |         |
|         |         |         |         |         | lozenge |         |
|         |         |         |         |         | .aui-   |         |
|         |         |         |         |         | lozenge |         |
|         |         |         |         |         | -subtle |         |
|         |         |         |         |         | .aui-l  |         |
|         |         |         |         |         | ozenge- |         |
|         |         |         |         |         | default |         |
|         |         |         |         |         | .issu   |         |
|         |         |         |         |         | e-place |         |
|         |         |         |         |         | holder} |         |
|         |         |         |         |         | ]{      |         |
|         |         |         |         |         | .conflu |         |
|         |         |         |         |         | ence-ji |         |
|         |         |         |         |         | m-macro |         |
|         |         |         |         |         | .jir    |         |
|         |         |         |         |         | a-issue |         |
|         |         |         |         |         | ji      |         |
|         |         |         |         |         | ra-key= |         |
|         |         |         |         |         | "WLT-1" |         |
|         |         |         |         |         | c       |         |
|         |         |         |         |         | lient-i |         |
|         |         |         |         |         | d="SING |         |
|         |         |         |         |         | LE_5581 |         |
|         |         |         |         |         | e30e-87 |         |
|         |         |         |         |         | 6a-3bbe |         |
|         |         |         |         |         | -9902-8 |         |
|         |         |         |         |         | 6eb613c |         |
|         |         |         |         |         | b022_24 |         |
|         |         |         |         |         | 9924812 |         |
|         |         |         |         |         | 9_5b142 |         |
|         |         |         |         |         | d79091e |         |
|         |         |         |         |         | 9f17116 |         |
|         |         |         |         |         | 363a5"} |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-8  | P       | Leave   | Shows   | [PASS]  |         | [YES]   |
|         | assword | p       | an      | {.statu |         | {.statu |
|         |         | assword | error   | s-macro |         | s-macro |
|         |         | field   | saying  | .aui-   |         | .aui-   |
|         |         | empty   | to      | lozenge |         | lozenge |
|         |         |         | enter   | .aui-lo |         | .aui-lo |
|         |         |         | wallet  | zenge-s |         | zenge-s |
|         |         |         | p       | uccess} |         | uccess} |
|         |         |         | assword |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-9  | T       | Enter   | T       | [PASS]  |         | [YES]   |
|         | ransfer | valid   | ransfer | {.statu |         | {.statu |
|         | xpx     | wallet  | tran    | s-macro |         | s-macro |
|         |         | a       | saction | .aui-   |         | .aui-   |
|         |         | ddress, | is      | lozenge |         | lozenge |
|         |         | valid   | succe   | .aui-lo |         | .aui-lo |
|         |         | t       | ssfully | zenge-s |         | zenge-s |
|         |         | ransfer | created | uccess} |         | uccess} |
|         |         | amount  |         |         |         |         |
|         |         | and     |         |         |         |         |
|         |         | correct |         |         |         |         |
|         |         | wallet  |         |         |         |         |
|         |         | pa      |         |         |         |         |
|         |         | ssword, |         |         |         |         |
|         |         | click   |         |         |         |         |
|         |         | t       |         |         |         |         |
|         |         | ransfer |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-10 |         | Enter   | Shows   | [PASS]  |         | [YES]   |
|         |         | valid   | an      | {.statu |         | {.statu |
|         |         | wallet  | error   | s-macro |         | s-macro |
|         |         | a       | saying  | .aui-   |         | .aui-   |
|         |         | ddress, | wallet  | lozenge |         | lozenge |
|         |         | valid   | p       | .aui-lo |         | .aui-lo |
|         |         | t       | assword | zenge-s |         | zenge-s |
|         |         | ransfer | is      | uccess} |         | uccess} |
|         |         | amount  | invalid |         |         |         |
|         |         | and     |         |         |         |         |
|         |         | in      |         |         |         |         |
|         |         | correct |         |         |         |         |
|         |         | wallet  |         |         |         |         |
|         |         | pa      |         |         |         |         |
|         |         | ssword, |         |         |         |         |
|         |         | click   |         |         |         |         |
|         |         | t       |         |         |         |         |
|         |         | ransfer |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-11 | T       | Click   | If      | [PASS]  |         | [YES]   |
|         | ransfer | to add  | amount  | {.statu |         | {.statu |
|         | Asset   | asset   | of      | s-macro |         | s-macro |
|         |         | for     | asset   | .aui-   |         | .aui-   |
|         |         | t       | entered | lozenge |         | lozenge |
|         |         | ransfer | exceeds | .aui-lo |         | .aui-lo |
|         |         |         | asset   | zenge-s |         | zenge-s |
|         |         |         | b       | uccess} |         | uccess} |
|         |         |         | alance, |         |         |         |
|         |         |         | an      |         |         |         |
|         |         |         | error   |         |         |         |
|         |         |         | is      |         |         |         |
|         |         |         | shown   |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-12 | Cancel  | Click   | User is | [PASS]  |         | [YES]   |
|         |         | on      | d       | {.statu |         | {.statu |
|         |         | cancel  | irected | s-macro |         | s-macro |
|         |         |         | back to | .aui-   |         | .aui-   |
|         |         |         | home    | lozenge |         | lozenge |
|         |         |         | page    | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-13 | Eye     | Click   | Sh      | [PASS]  |         | [YES]   |
|         | icon    | on eye  | ow/hide | {.statu |         | {.statu |
|         |         | icon    | p       | s-macro |         | s-macro |
|         |         | beside  | assword | .aui-   |         | .aui-   |
|         |         | p       |         | lozenge |         | lozenge |
|         |         | assword |         | .aui-lo |         | .aui-lo |
|         |         | field   |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
:::

::: table-wrap
+---------+---------+---------+---------+---------+---------+---------+
| ## Acco |         |         |         |         |         |         |
| unts {# |         |         |         |         |         |         |
| TestRep |         |         |         |         |         |         |
| ort-1.1 |         |         |         |         |         |         |
| .8-1-Ac |         |         |         |         |         |         |
| counts} |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| **Test  | **Test  | **Test  | **E     | **S     | **R     | **Auto  |
| Case    | Scen    | steps** | xpected | tatus** | emark** | mated** |
| ID**    | arios** |         | r       |         |         |         |
|         |         |         | esult** |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCTS-1 | Create  | Click   | Go to   | [PASS]  |         | [YES]   |
|         | a New   | "Create | "       | {.statu |         | {.statu |
|         | Account | New     | Account | s-macro |         | s-macro |
|         |         | A       | \>      | .aui-   |         | .aui-   |
|         |         | ccount" | +Create | lozenge |         | lozenge |
|         |         |         | New     | .aui-lo |         | .aui-lo |
|         |         |         | Account | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| ACCTS-2 | Account | Click   | Go to   | [PASS]  |         | [YES]   |
|         | Details | on any  | "       | {.statu |         | {.statu |
|         |         | account | Account | s-macro |         | s-macro |
|         |         | under   | \>      | .aui-   |         | .aui-   |
|         |         | A       | D       | lozenge |         | lozenge |
|         |         | ccounts | etails" | .aui-lo |         | .aui-lo |
|         |         | \>      | page    | zenge-s |         | zenge-s |
|         |         | Details |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| ACCTS-3 | Make as | Click   | Account | [PASS]  |         | [YES]   |
|         | Default | on      | Av      | {.statu |         | {.statu |
|         |         | default | ailable | s-macro |         | s-macro |
|         |         | button  | pop up  | .aui-   |         | .aui-   |
|         |         | beside  | will    | lozenge |         | lozenge |
|         |         | DEFAULT | show    | .aui-lo |         | .aui-lo |
|         |         | ACCOUNT | up,     | zenge-s |         | zenge-s |
|         |         |         | user    | uccess} |         | uccess} |
|         |         |         | can     |         |         |         |
|         |         |         | select  |         |         |         |
|         |         |         | which   |         |         |         |
|         |         |         | account |         |         |         |
|         |         |         | to be   |         |         |         |
|         |         |         | chosen  |         |         |         |
|         |         |         | as      |         |         |         |
|         |         |         | default |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCTS-4 | Export  | Click   | Account | [PASS]  |         | [YES]   |
|         | Account | on      | will be | {.statu |         | {.statu |
|         |         | export  | e       | s-macro |         | s-macro |
|         |         | button  | xported | .aui-   |         | .aui-   |
|         |         | under   | to      | lozenge |         | lozenge |
|         |         | wallets | local   | .aui-lo |         | .aui-lo |
|         |         |         | machine | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| ACCTS-5 | Delete  | Click   | Prompt  | [PASS]  |         | [YES]   |
|         | an      | on      | for     | {.statu |         | {.statu |
|         | Account | "Delete | confi   | s-macro |         | s-macro |
|         |         | This    | rmation | .aui-   |         | .aui-   |
|         |         | A       | to      | lozenge |         | lozenge |
|         |         | ccount" | delete  | .aui-lo |         | .aui-lo |
|         |         | button  | the     | zenge-s |         | zenge-s |
|         |         |         | a       | uccess} |         | uccess} |
|         |         |         | ccount, |         |         |         |
|         |         |         | p       |         |         |         |
|         |         |         | assword |         |         |         |
|         |         |         | is      |         |         |         |
|         |         |         | r       |         |         |         |
|         |         |         | equired |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCTS-6 |         | Enter   | Account | [PASS]  |         | [YES]   |
|         |         | Correct | succe   | {.statu |         | {.statu |
|         |         | Account | ssfully | s-macro |         | s-macro |
|         |         | Pas     | removed | .aui-   |         | .aui-   |
|         |         | sword,\ | with a  | lozenge |         | lozenge |
|         |         | Click   | notif   | .aui-lo |         | .aui-lo |
|         |         | "       | ication | zenge-s |         | zenge-s |
|         |         | Confirm | p       | uccess} |         | uccess} |
|         |         | De      | rompted |         |         |         |
|         |         | letion" | for     |         |         |         |
|         |         |         | user    |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCTS-7 |         | Enter   | User is | [PASS]  |         | [YES]   |
|         |         | Correct | d       | {.statu |         | {.statu |
|         |         | Account | irected | s-macro |         | s-macro |
|         |         | Pas     | back to | .aui-   |         | .aui-   |
|         |         | sword,\ | account | lozenge |         | lozenge |
|         |         | Click   | details | .aui-lo |         | .aui-lo |
|         |         | "       | page    | zenge-s |         | zenge-s |
|         |         | Cancel" |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| ACCTS-8 |         | Enter   | An      | [PASS]  |         | [YES]   |
|         |         | In      | error   | {.statu |         | {.statu |
|         |         | correct | is      | s-macro |         | s-macro |
|         |         | Account | shown   | .aui-   |         | .aui-   |
|         |         | Pas     |         | lozenge |         | lozenge |
|         |         | sword,\ |         | .aui-lo |         | .aui-lo |
|         |         | Click   |         | zenge-s |         | zenge-s |
|         |         | "       |         | uccess} |         | uccess} |
|         |         | Confirm |         |         |         |         |
|         |         | De      |         |         |         |         |
|         |         | letion" |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCTS-9 | Eye     | Click   | Sh      | [PASS]  |         | [YES]   |
|         | icon    | on      | ow/hide | {.statu |         | {.statu |
|         |         | p       | p       | s-macro |         | s-macro |
|         |         | assword | assword | .aui-   |         | .aui-   |
|         |         | eye     |         | lozenge |         | lozenge |
|         |         | icon    |         | .aui-lo |         | .aui-lo |
|         |         | when    |         | zenge-s |         | zenge-s |
|         |         | d       |         | uccess} |         | uccess} |
|         |         | eleting |         |         |         |         |
|         |         | account |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| A       | Labels  | Click   | A drop  | [PASS]  |         |         |
| CCTS-10 |         | on      | down    | {.statu |         |         |
|         |         | "       | list of | s-macro |         |         |
|         |         | Labels" | labels  | .aui-   |         |         |
|         |         | on      | will    | lozenge |         |         |
|         |         | A       | appear  | .aui-lo |         |         |
|         |         | ccounts |         | zenge-s |         |         |
|         |         | page    |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| A       |         | Click   | Create  | [PASS]  |         |         |
| CCTS-11 |         | on "+   | Label   | {.statu |         |         |
|         |         | Create  | pop up  | s-macro |         |         |
|         |         | Label"  | dialog  | .aui-   |         |         |
|         |         |         | will    | lozenge |         |         |
|         |         |         | appear  | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| A       |         | Leave   | An      | [PASS]  |         |         |
| CCTS-12 |         | label   | error   | {.statu |         |         |
|         |         | name    | is      | s-macro |         |         |
|         |         | empty   | shown   | .aui-   |         |         |
|         |         |         | saying  | lozenge |         |         |
|         |         |         | label   | .aui-lo |         |         |
|         |         |         | name    | zenge-s |         |         |
|         |         |         | cannot  | uccess} |         |         |
|         |         |         | be      |         |         |         |
|         |         |         | empty   |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| A       |         | Enter   | User is | [PASS]  |         |         |
| CCTS-13 |         | label   | d       | {.statu |         |         |
|         |         | name,   | irected | s-macro |         |         |
|         |         | click   | back to | .aui-   |         |         |
|         |         | "       | account | lozenge |         |         |
|         |         | Cancel" | page    | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| A       |         | Enter   | Label   | [PASS]  |         |         |
| CCTS-14 |         | label   | name is | {.statu |         |         |
|         |         | name,   | succe   | s-macro |         |         |
|         |         | click   | ssfully | .aui-   |         |         |
|         |         | "C      | created | lozenge |         |         |
|         |         | onfirm" | with a  | .aui-lo |         |         |
|         |         |         | notif   | zenge-s |         |         |
|         |         |         | ication | uccess} |         |         |
|         |         |         | p       |         |         |         |
|         |         |         | rompted |         |         |         |
|         |         |         | for     |         |         |         |
|         |         |         | user    |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| A       |         | Click   | Label   | [PASS]  |         |         |
| CCTS-15 |         | on      | is      | {.statu |         |         |
|         |         | trash   | removed | s-macro |         |         |
|         |         | button  | with a  | .aui-   |         |         |
|         |         |         | notif   | lozenge |         |         |
|         |         |         | ication | .aui-lo |         |         |
|         |         |         | p       | zenge-s |         |         |
|         |         |         | rompted | uccess} |         |         |
|         |         |         | for     |         |         |         |
|         |         |         | user    |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| A       | Adding  | Click   | Shows a | [PASS]  |         |         |
| CCTS-16 | labels  | on      | notif   | {.statu |         |         |
|         | on      | "..."   | ication | s-macro |         |         |
|         | account | button  | saying  | .aui-   |         |         |
|         |         | for     | that    | lozenge |         |         |
|         |         | a       | "       | .aui-lo |         |         |
|         |         | ccount, | account | zenge-s |         |         |
|         |         | click   | name"   | uccess} |         |         |
|         |         | on      | is      |         |         |         |
|         |         | s       | added   |         |         |         |
|         |         | pecific | as      |         |         |         |
|         |         | label   | "label  |         |         |         |
|         |         |         | name"   |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| A       | R       | Click   | Shows a | [PASS]  |         |         |
| CCTS-17 | emoving | on      | notif   | {.statu |         |         |
|         | labels  | "..."   | ication | s-macro |         |         |
|         | from    | button  | saying  | .aui-   |         |         |
|         | account | for     | that    | lozenge |         |         |
|         |         | a       | "       | .aui-lo |         |         |
|         |         | ccount, | account | zenge-s |         |         |
|         |         | click   | name"   | uccess} |         |         |
|         |         | on the  | is      |         |         |         |
|         |         | same    | removed |         |         |         |
|         |         | label   | as      |         |         |         |
|         |         |         | "label  |         |         |         |
|         |         |         | name"   |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| A       | label   | Click   | Account | [PASS]  |         |         |
| CCTS-18 | filter  | on      | will be | {.statu |         |         |
|         |         | s       | f       | s-macro |         |         |
|         |         | pecific | iltered | .aui-   |         |         |
|         |         | label   | based   | lozenge |         |         |
|         |         | on      | on      | .aui-lo |         |         |
|         |         | label   | label   | zenge-s |         |         |
|         |         | d       |         | uccess} |         |         |
|         |         | ropdown |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| A       | Dese    | Click   | Label   | [PASS]  |         |         |
| CCTS-19 | lecting | on      | gets    | {.statu |         |         |
|         | label   | s       | des     | s-macro |         |         |
|         | filter  | elected | elected | .aui-   |         |         |
|         |         | label   | and     | lozenge |         |         |
|         |         | on      | will    | .aui-lo |         |         |
|         |         | label   | show    | zenge-s |         |         |
|         |         | d       | all     | uccess} |         |         |
|         |         | ropdown | account |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ##      |         |         |         |         |         |         |
| # Selec |         |         |         |         |         |         |
| t Creat |         |         |         |         |         |         |
| ion Typ |         |         |         |         |         |         |
| e {#Tes |         |         |         |         |         |         |
| tReport |         |         |         |         |         |         |
| -1.1.8- |         |         |         |         |         |         |
| 1-Selec |         |         |         |         |         |         |
| tCreati |         |         |         |         |         |         |
| onType} |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| N       | Create  | Click   | Go to   | [PASS]  |         | [YES]   |
| EWACC-1 | New     | on      | "Create | {.statu |         | {.statu |
|         |         | "Create | New     | s-macro |         | s-macro |
|         |         | New"    | A       | .aui-   |         | .aui-   |
|         |         | button  | ccount" | lozenge |         | lozenge |
|         |         |         | Page    | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| N       | From a  | Click   | Go to   | [PASS]  |         | [YES]   |
| EWACC-2 | Private | on      | "Create | {.statu |         | {.statu |
|         | Key     | "From a | New     | s-macro |         | s-macro |
|         |         | Private | Account | .aui-   |         | .aui-   |
|         |         | Key"    | From    | lozenge |         | lozenge |
|         |         | button  | Private | .aui-lo |         | .aui-lo |
|         |         |         | Key"    | zenge-s |         | zenge-s |
|         |         |         | Page    | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| #       |         |         |         |         |         |         |
| ### Cre |         |         |         |         |         |         |
| ate a N |         |         |         |         |         |         |
| ew Acco |         |         |         |         |         |         |
| unt in  |         |         |         |         |         |         |
| the sam |         |         |         |         |         |         |
| e Walle |         |         |         |         |         |         |
| t {#Tes |         |         |         |         |         |         |
| tReport |         |         |         |         |         |         |
| -1.1.8- |         |         |         |         |         |         |
| 1-Creat |         |         |         |         |         |         |
| eaNewAc |         |         |         |         |         |         |
| countin |         |         |         |         |         |         |
| thesame |         |         |         |         |         |         |
| Wallet} |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| N       | Create  | Cu      | Go to   | [PASS]  |         | [YES]   |
| EWACC-3 | a New   | rrently | "Select | {.statu |         | {.statu |
|         | Account | in      | C       | s-macro |         | s-macro |
|         |         | "Create | reation | .aui-   |         | .aui-   |
|         |         | New     | Type"   | lozenge |         | lozenge |
|         |         | A       |         | .aui-lo |         | .aui-lo |
|         |         | ccount" |         | zenge-s |         | zenge-s |
|         |         | page    |         | uccess} |         | uccess} |
|         |         | and     |         |         |         |         |
|         |         | click   |         |         |         |         |
|         |         | "Back"  |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| N       |         | Leave   | Show a  | [PASS]  |         | [YES]   |
| EWACC-4 |         | account | message | {.statu |         | {.statu |
|         |         | name    | "Enter  | s-macro |         | s-macro |
|         |         | empty   | Account | .aui-   |         | .aui-   |
|         |         |         | Name"   | lozenge |         | lozenge |
|         |         |         |         | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| N       |         | Enter   | Show a  | [PASS]  |         | [YES]   |
| EWACC-5 |         | Account | message | {.statu |         | {.statu |
|         |         | Name,\  | "min    | s-macro |         | s-macro |
|         |         | Leave   | length  | .aui-   |         | .aui-   |
|         |         | p       | 8",     | lozenge |         | lozenge |
|         |         | assword | unable  | .aui-lo |         | .aui-lo |
|         |         | field   | to      | zenge-s |         | zenge-s |
|         |         | empty   | create  | uccess} |         | uccess} |
|         |         |         | account |         |         |         |
|         |         |         | (create |         |         |         |
|         |         |         | button  |         |         |         |
|         |         |         | di      |         |         |         |
|         |         |         | sabled) |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| N       |         | Enter   | Show a  | [PASS]  |         | [YES]   |
| EWACC-6 |         | Account | message | {.statu |         | {.statu |
|         |         | Name,\  | "P      | s-macro |         | s-macro |
|         |         | Enter   | assword | .aui-   |         | .aui-   |
|         |         | in      | for     | lozenge |         | lozenge |
|         |         | correct | wallet  | .aui-lo |         | .aui-lo |
|         |         | Wallet  | \<name  | zenge-s |         | zenge-s |
|         |         | Pa      | of      | uccess} |         | uccess} |
|         |         | ssword\ | w       |         |         |         |
|         |         | Click   | allet\> |         |         |         |
|         |         | "       | is      |         |         |         |
|         |         | Create" | i       |         |         |         |
|         |         |         | nvalid" |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| N       |         | Enter   | Send a  | [PASS]  |         | [YES]   |
| EWACC-7 |         | Account | confi   | {.statu |         | {.statu |
|         |         | Name,\  | rmation | s-macro |         | s-macro |
|         |         | Enter   | message | .aui-   |         | .aui-   |
|         |         | Correct | and     | lozenge |         | lozenge |
|         |         | Wallet  | create  | .aui-lo |         | .aui-lo |
|         |         | Pa      | the     | zenge-s |         | zenge-s |
|         |         | ssword\ | account | uccess} |         | uccess} |
|         |         | Click   |         |         |         |         |
|         |         | "       |         |         |         |         |
|         |         | Create" |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| N       | Eye     | Click   | Sh      | [PASS]  |         | [YES]   |
| EWACC-8 | icon    | on      | ow/hide | {.statu |         | {.statu |
|         |         | "Pa     | p       | s-macro |         | s-macro |
|         |         | ssword" | assword | .aui-   |         | .aui-   |
|         |         | eye     |         | lozenge |         | lozenge |
|         |         | icon    |         | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| ####    |         |         |         |         |         |         |
|  Create |         |         |         |         |         |         |
|  a New  |         |         |         |         |         |         |
| Account |         |         |         |         |         |         |
|  from P |         |         |         |         |         |         |
| rivate  |         |         |         |         |         |         |
| Key in  |         |         |         |         |         |         |
| the sam |         |         |         |         |         |         |
| e Walle |         |         |         |         |         |         |
| t {#Tes |         |         |         |         |         |         |
| tReport |         |         |         |         |         |         |
| -1.1.8- |         |         |         |         |         |         |
| 1-Creat |         |         |         |         |         |         |
| eaNewAc |         |         |         |         |         |         |
| countfr |         |         |         |         |         |         |
| omPriva |         |         |         |         |         |         |
| teKeyin |         |         |         |         |         |         |
| thesame |         |         |         |         |         |         |
| Wallet} |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| N       | Create  | Cu      | Go to   | [PASS]  |         | [YES]   |
| EWACC-9 | a New   | rrently | "Select | {.statu |         | {.statu |
|         | Account | in      | C       | s-macro |         | s-macro |
|         | from    | "Create | reation | .aui-   |         | .aui-   |
|         | Private | New     | Type"   | lozenge |         | lozenge |
|         | Key     | Account |         | .aui-lo |         | .aui-lo |
|         |         | From    |         | zenge-s |         | zenge-s |
|         |         | Private |         | uccess} |         | uccess} |
|         |         | Key"    |         |         |         |         |
|         |         | page    |         |         |         |         |
|         |         | and     |         |         |         |         |
|         |         | click   |         |         |         |         |
|         |         | "Back"  |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Leave   | Show a  | [PASS]  |         | [YES]   |
| WACC-10 |         | Private | message | {.statu |         | {.statu |
|         |         | Key     | "       | s-macro |         | s-macro |
|         |         | empty   | Invalid | .aui-   |         | .aui-   |
|         |         |         | Private | lozenge |         | lozenge |
|         |         |         | Key"    | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Enter   | Show a  | [PASS]  |         | [YES]   |
| WACC-11 |         | Private | message | {.statu |         | {.statu |
|         |         | Key,\   | "Enter  | s-macro |         | s-macro |
|         |         | Leave   | Wallet  | .aui-   |         | .aui-   |
|         |         | Account | Name"   | lozenge |         | lozenge |
|         |         | Name    |         | .aui-lo |         | .aui-lo |
|         |         | empty   |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Enter   | Show a  | [PASS]  |         | [YES]   |
| WACC-12 |         | Private | message | {.statu |         | {.statu |
|         |         | Key,\   | "p      | s-macro |         | s-macro |
|         |         | Enter   | assword | .aui-   |         | .aui-   |
|         |         | Account | is      | lozenge |         | lozenge |
|         |         | Name,\  | req     | .aui-lo |         | .aui-lo |
|         |         | Leave   | uired", | zenge-s |         | zenge-s |
|         |         | p       | unable  | uccess} |         | uccess} |
|         |         | assword | to      |         |         |         |
|         |         | field   | create  |         |         |         |
|         |         | empty   | account |         |         |         |
|         |         |         | (create |         |         |         |
|         |         |         | button  |         |         |         |
|         |         |         | di      |         |         |         |
|         |         |         | sabled) |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Enter   | Show a  | [PASS]  |         | [YES]   |
| WACC-13 |         | Private | message | {.statu |         | {.statu |
|         |         | Key,\   | "P      | s-macro |         | s-macro |
|         |         | Enter   | assword | .aui-   |         | .aui-   |
|         |         | Account | for     | lozenge |         | lozenge |
|         |         | Name,\  | wallet  | .aui-lo |         | .aui-lo |
|         |         | Enter   | \<name  | zenge-s |         | zenge-s |
|         |         | in      | of      | uccess} |         | uccess} |
|         |         | correct | w       |         |         |         |
|         |         | wallet  | allet\> |         |         |         |
|         |         | pa      | is      |         |         |         |
|         |         | ssword\ | i       |         |         |         |
|         |         | Click   | nvalid" |         |         |         |
|         |         | "       |         |         |         |         |
|         |         | Create" |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Enter   | Send a  | [PASS]  |         | [YES]   |
| WACC-14 |         | Private | confi   | {.statu |         | {.statu |
|         |         | Key,\   | rmation | s-macro |         | s-macro |
|         |         | Enter   | message | .aui-   |         | .aui-   |
|         |         | Account | and     | lozenge |         | lozenge |
|         |         | Name,\  | create  | .aui-lo |         | .aui-lo |
|         |         | Enter   | the     | zenge-s |         | zenge-s |
|         |         | correct | account | uccess} |         | uccess} |
|         |         | wallet  |         |         |         |         |
|         |         | pa      |         |         |         |         |
|         |         | ssword\ |         |         |         |         |
|         |         | Click   |         |         |         |         |
|         |         | "       |         |         |         |         |
|         |         | Create" |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      | Eye     | Click   | Sh      | [PASS]  |         | [YES]   |
| WACC-15 | icon    | on      | ow/hide | {.statu |         | {.statu |
|         |         | "Pa     | p       | s-macro |         | s-macro |
|         |         | ssword" | assword | .aui-   |         | .aui-   |
|         |         | eye     |         | lozenge |         | lozenge |
|         |         | icon    |         | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| ##      |         |         |         |         |         |         |
| # Edit  |         |         |         |         |         |         |
| an exis |         |         |         |         |         |         |
| ting Ac |         |         |         |         |         |         |
| count { |         |         |         |         |         |         |
| #TestRe |         |         |         |         |         |         |
| port-1. |         |         |         |         |         |         |
| 1.8-1-E |         |         |         |         |         |         |
| ditanex |         |         |         |         |         |         |
| istingA |         |         |         |         |         |         |
| ccount} |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| #### De |         |         |         |         |         |         |
| tails { |         |         |         |         |         |         |
| #TestRe |         |         |         |         |         |         |
| port-1. |         |         |         |         |         |         |
| 1.8-1-D |         |         |         |         |         |         |
| etails} |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCDE   | Change  | Click   | Account | [PASS]  |         | [YES]   |
| TAILS-1 | Account | on      | name    | {.statu |         | {.statu |
|         | Name    | "       | updated | s-macro |         | s-macro |
|         |         | Pencil" | and     | .aui-   |         | .aui-   |
|         |         | icon    | re      | lozenge |         | lozenge |
|         |         | beside  | flected | .aui-lo |         | .aui-lo |
|         |         | Account | under   | zenge-s |         | zenge-s |
|         |         | Name,   | the     | uccess} |         | uccess} |
|         |         | enter   | "Ac     |         |         |         |
|         |         | new     | counts" |         |         |         |
|         |         | account | side    |         |         |         |
|         |         | name    | bar     |         |         |         |
|         |         | and     |         |         |         |         |
|         |         | click   |         |         |         |         |
|         |         | the     |         |         |         |         |
|         |         | "pencil |         |         |         |         |
|         |         | icon"   |         |         |         |         |
|         |         | again   |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCDE   | Copy    | Click   | Wallet  | [PASS]  |         | [YES]   |
| TAILS-2 | Wallet  | "Copy"  | Address | {.statu |         | {.statu |
|         | Address | icon    | is      | s-macro |         | s-macro |
|         |         | under   | copied  | .aui-   |         | .aui-   |
|         |         | Wallet  | to      | lozenge |         | lozenge |
|         |         | Address | user's  | .aui-lo |         | .aui-lo |
|         |         |         | cl      | zenge-s |         | zenge-s |
|         |         |         | ipboard | uccess} |         | uccess} |
|         |         |         | and a   |         |         |         |
|         |         |         | notif   |         |         |         |
|         |         |         | ication |         |         |         |
|         |         |         | is      |         |         |         |
|         |         |         | shown   |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCDE   | Copy    | Click   | Public  | [PASS]  |         | [YES]   |
| TAILS-3 | Public  | "Copy"  | Key is  | {.statu |         | {.statu |
|         | Key     | icon    | copied  | s-macro |         | s-macro |
|         |         | under   | to      | .aui-   |         | .aui-   |
|         |         | Public  | user's  | lozenge |         | lozenge |
|         |         | Key     | cl      | .aui-lo |         | .aui-lo |
|         |         |         | ipboard | zenge-s |         | zenge-s |
|         |         |         | and a   | uccess} |         | uccess} |
|         |         |         | notif   |         |         |         |
|         |         |         | ication |         |         |         |
|         |         |         | is      |         |         |         |
|         |         |         | shown   |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCDE   | Show    | Click   | Prompt  | [PASS]  |         | [YES]   |
| TAILS-4 | Private | on      | for     | {.statu |         | {.statu |
|         | Key     | "       | user to | s-macro |         | s-macro |
|         |         | Private | enter   | .aui-   |         | .aui-   |
|         |         | Key"    | p       | lozenge |         | lozenge |
|         |         | eye     | assword | .aui-lo |         | .aui-lo |
|         |         | icon\   |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| ACCDE   |         | Enter   | Private | [PASS]  |         | [YES]   |
| TAILS-5 |         | correct | Key is  | {.statu |         | {.statu |
|         |         | wallet  | visible | s-macro |         | s-macro |
|         |         | pa      | and     | .aui-   |         | .aui-   |
|         |         | ssword\ | allows  | lozenge |         | lozenge |
|         |         | Click   | user to | .aui-lo |         | .aui-lo |
|         |         | "C      | copy it | zenge-s |         | zenge-s |
|         |         | onfirm" |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| ACCDE   |         | Enter   | Go back | [PASS]  |         | [YES]   |
| TAILS-6 |         | correct | to      | {.statu |         | {.statu |
|         |         | wallet  | Account | s-macro |         | s-macro |
|         |         | pa      | Details | .aui-   |         | .aui-   |
|         |         | ssword\ | page    | lozenge |         | lozenge |
|         |         | Click   |         | .aui-lo |         | .aui-lo |
|         |         | "       |         | zenge-s |         | zenge-s |
|         |         | Cancel" |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| ACCDE   |         | Enter   | Show a  | [PASS]  |         | [YES]   |
| TAILS-7 |         | in      | message | {.statu |         | {.statu |
|         |         | correct | "Wallet | s-macro |         | s-macro |
|         |         | wallet  | p       | .aui-   |         | .aui-   |
|         |         | pa      | assword | lozenge |         | lozenge |
|         |         | ssword\ | is      | .aui-lo |         | .aui-lo |
|         |         | Click   | inc     | zenge-s |         | zenge-s |
|         |         | "C      | orrect" | uccess} |         | uccess} |
|         |         | onfirm" |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCDE   |         | Enter   | Show a  | [PASS]  |         | [YES]   |
| TAILS-8 |         | blank   | message | {.statu |         | {.statu |
|         |         | wallet  | "P      | s-macro |         | s-macro |
|         |         | pa      | assword | .aui-   |         | .aui-   |
|         |         | ssword\ | is      | lozenge |         | lozenge |
|         |         | Click   | re      | .aui-lo |         | .aui-lo |
|         |         | "C      | quired" | zenge-s |         | zenge-s |
|         |         | onfirm" |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| ACCDE   | Copy    | Click   | Private | [PASS]  |         | [YES]   |
| TAILS-9 | Private | "Copy"  | Key is  | {.statu |         | {.statu |
|         | Key     | icon    | copied  | s-macro |         | s-macro |
|         |         | under   | to      | .aui-   |         | .aui-   |
|         |         | Private | user's  | lozenge |         | lozenge |
|         |         | Key     | cl      | .aui-lo |         | .aui-lo |
|         |         | after   | ipboard | zenge-s |         | zenge-s |
|         |         | it is   | and a   | uccess} |         | uccess} |
|         |         | shown   | notif   |         |         |         |
|         |         |         | ication |         |         |         |
|         |         |         | is      |         |         |         |
|         |         |         | shown   |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCDET  | D       | Click   | Prompt  | [PASS]  |         | [YES]   |
| AILS-10 | ownload | on      | for     | {.statu |         | {.statu |
|         | Wallet  | "D      | user to | s-macro |         | s-macro |
|         | Paper   | ownload | enter   | .aui-   |         | .aui-   |
|         |         | Wallet  | wallet  | lozenge |         | lozenge |
|         |         | Paper"  | p       | .aui-lo |         | .aui-lo |
|         |         | button  | assword | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| ACCDET  |         | Enter   | User's  | [PASS]  |         |         |
| AILS-11 |         | correct | wallet  | {.statu |         |         |
|         |         | wallet  | paper   | s-macro |         |         |
|         |         | pa      | dow     | .aui-   |         |         |
|         |         | ssword\ | nloaded | lozenge |         |         |
|         |         | Click   | to      | .aui-lo |         |         |
|         |         | "C      | their   | zenge-s |         |         |
|         |         | onfirm" | local   | uccess} |         |         |
|         |         |         | machine |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCDET  |         | Enter   | Go back | [PASS]  |         | [YES]   |
| AILS-12 |         | correct | to      | {.statu |         | {.statu |
|         |         | wallet  | Account | s-macro |         | s-macro |
|         |         | pa      | Details | .aui-   |         | .aui-   |
|         |         | ssword\ | page    | lozenge |         | lozenge |
|         |         | Click   |         | .aui-lo |         | .aui-lo |
|         |         | "       |         | zenge-s |         | zenge-s |
|         |         | Cancel" |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| ACCDET  |         | Enter   | Show a  | [PASS]  |         | [YES]   |
| AILS-13 |         | in      | message | {.statu |         | {.statu |
|         |         | correct | "Wallet | s-macro |         | s-macro |
|         |         | wallet  | p       | .aui-   |         | .aui-   |
|         |         | pa      | assword | lozenge |         | lozenge |
|         |         | ssword\ | is      | .aui-lo |         | .aui-lo |
|         |         | Click   | inc     | zenge-s |         | zenge-s |
|         |         | "C      | orrect" | uccess} |         | uccess} |
|         |         | onfirm" |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCDET  |         | Enter   | Show a  | [PASS]  |         | [YES]   |
| AILS-14 |         | blank   | message | {.statu |         | {.statu |
|         |         | wallet  | "P      | s-macro |         | s-macro |
|         |         | pa      | assword | .aui-   |         | .aui-   |
|         |         | ssword\ | is      | lozenge |         | lozenge |
|         |         | Click   | re      | .aui-lo |         | .aui-lo |
|         |         | "C      | quired" | zenge-s |         | zenge-s |
|         |         | onfirm" |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| ACCDET  | Eye     | Click   | Sh      | [PASS]  |         | [YES]   |
| AILS-15 | icon    | on      | ow/hide | {.statu |         | {.statu |
|         |         | p       | p       | s-macro |         | s-macro |
|         |         | assword | assword | .aui-   |         | .aui-   |
|         |         | eye     |         | lozenge |         | lozenge |
|         |         | icon    |         | .aui-lo |         | .aui-lo |
|         |         | when    |         | zenge-s |         | zenge-s |
|         |         | e       |         | uccess} |         | uccess} |
|         |         | ntering |         |         |         |         |
|         |         | wallet  |         |         |         |         |
|         |         | p       |         |         |         |         |
|         |         | assword |         |         |         |         |
|         |         | to show |         |         |         |         |
|         |         | private |         |         |         |         |
|         |         | key     |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCDET  |         | Click   | Hide    | [PASS]  |         | [YES]   |
| AILS-16 |         | on hide | private | {.statu |         | {.statu |
|         |         | private | key     | s-macro |         | s-macro |
|         |         | key eye |         | .aui-   |         | .aui-   |
|         |         | icon to |         | lozenge |         | lozenge |
|         |         | mask it |         | .aui-lo |         | .aui-lo |
|         |         | again   |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| ACCDET  | D       | Go to   | Account | [PASS]  |         | [YES]   |
| AILS-17 | elegate | "A      | is      | {.statu |         | {.statu |
|         |         | ccounts | linked  | s-macro |         | s-macro |
|         |         | \>      | to a    | .aui-   |         | .aui-   |
|         |         | Del     | de      | lozenge |         | lozenge |
|         |         | egate"\ | legated | .aui-lo |         | .aui-lo |
|         |         | Select  | a       | zenge-s |         | zenge-s |
|         |         | a       | ccount\ | uccess} |         | uccess} |
|         |         | linking | Public  |         |         |         |
|         |         | a       | and     |         |         |         |
|         |         | ccount\ | private |         |         |         |
|         |         | Account | keys    |         |         |         |
|         |         | type as | av      |         |         |         |
|         |         | "New    | ailable |         |         |         |
|         |         | A       | for     |         |         |         |
|         |         | ccount" | user to |         |         |         |
|         |         | or      | store   |         |         |         |
|         |         | "From a |         |         |         |         |
|         |         | Private |         |         |         |         |
|         |         | Key"    |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCDET  |         | Click   | De      | [PASS]  |         | [YES]   |
| AILS-18 |         | "Save   | legated | {.statu |         | {.statu |
|         |         | as      | ac      | s-macro |         | s-macro |
|         |         | Wallet  | count's | .aui-   |         | .aui-   |
|         |         | Paper"  | wallet  | lozenge |         | lozenge |
|         |         | button  | paper   | .aui-lo |         | .aui-lo |
|         |         |         | dow     | zenge-s |         | zenge-s |
|         |         |         | nloaded | uccess} |         | uccess} |
|         |         |         | to      |         |         |         |
|         |         |         | user's  |         |         |         |
|         |         |         | local   |         |         |         |
|         |         |         | machine |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCDET  |         | Click   | Go back | [PASS]  |         | [YES]   |
| AILS-19 |         | "C      | to      | {.statu |         | {.statu |
|         |         | ontinue | A       | s-macro |         | s-macro |
|         |         |         | ccounts | .aui-   |         | .aui-   |
|         |         |         | \> View | lozenge |         | lozenge |
|         |         |         | All     | .aui-lo |         | .aui-lo |
|         |         |         | page    | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| ### Con |         |         |         |         |         |         |
| vert to |         |         |         |         |         |         |
|  Multis |         |         |         |         |         |         |
| ig {#Te |         |         |         |         |         |         |
| stRepor |         |         |         |         |         |         |
| t-1.1.8 |         |         |         |         |         |         |
| -1-Conv |         |         |         |         |         |         |
| erttoMu |         |         |         |         |         |         |
| ltisig} |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| CV      | Convert | Click   | If      | [PASS]  |         |         |
| TMTSG-1 | to      | to      | account | {.statu |         |         |
|         | M       | Account | has     | s-macro |         |         |
|         | ultisig | \>      | insuf   | .aui-   |         |         |
|         |         | M       | ficient | lozenge |         |         |
|         |         | ultisig | xpx (0  | .aui-lo |         |         |
|         |         |         | xpx),   | zenge-s |         |         |
|         |         |         | an      | uccess} |         |         |
|         |         |         | error   |         |         |         |
|         |         |         | message |         |         |         |
|         |         |         | is      |         |         |         |
|         |         |         | shown   |         |         |         |
|         |         |         | and     |         |         |         |
|         |         |         | could   |         |         |         |
|         |         |         | not     |         |         |         |
|         |         |         | proceed |         |         |         |
|         |         |         | to      |         |         |         |
|         |         |         | convert |         |         |         |
|         |         |         | to      |         |         |         |
|         |         |         | M       |         |         |         |
|         |         |         | ultisig |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| CV      | Scheme  | Add and | Value   | [PASS]  |         |         |
| TMTSG-2 |         | reduce  | does    | {.statu |         |         |
|         |         | approve | not     | s-macro |         |         |
|         |         | trans   | exceed  | .aui-   |         |         |
|         |         | actions | max     | lozenge |         |         |
|         |         |         | number  | .aui-lo |         |         |
|         |         |         | of      | zenge-s |         |         |
|         |         |         | cosigna | uccess} |         |         |
|         |         |         | tories, |         |         |         |
|         |         |         | and     |         |         |         |
|         |         |         | error   |         |         |         |
|         |         |         | is      |         |         |         |
|         |         |         | shown   |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| CV      |         | Add and | Value   | [PASS]  |         |         |
| TMTSG-3 |         | reduce  | does    | {.statu |         |         |
|         |         | delete  | not     | s-macro |         |         |
|         |         | users   | exceed  | .aui-   |         |         |
|         |         |         | max     | lozenge |         |         |
|         |         |         | number  | .aui-lo |         |         |
|         |         |         | of      | zenge-s |         |         |
|         |         |         | cosigna | uccess} |         |         |
|         |         |         | tories, |         |         |         |
|         |         |         | and     |         |         |         |
|         |         |         | error   |         |         |         |
|         |         |         | is      |         |         |         |
|         |         |         | shown   |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| CV      | Add     | Click   | Opens   | [PASS]  |         |         |
| TMTSG-4 | Cosi    | M       | up      | {.statu |         |         |
|         | gnatory | ultisig | M       | s-macro |         |         |
|         |         | tab     | ultisig | .aui-   |         |         |
|         |         | under   | S       | lozenge |         |         |
|         |         | a       | ettings | .aui-lo |         |         |
|         |         | ccounts |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| CV      |         | Click   | User is | [PASS]  |         |         |
| TMTSG-5 |         | "Manage | d       | {.statu |         |         |
|         |         | Cosigna | irected | s-macro |         |         |
|         |         | tories" | to      | .aui-   |         |         |
|         |         | button  | convert | lozenge |         |         |
|         |         | under   | account | .aui-lo |         |         |
|         |         | Account | to      | zenge-s |         |         |
|         |         | \>      | m       | uccess} |         |         |
|         |         | M       | ultisig |         |         |         |
|         |         | ultisig | page    |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| CV      |         | Click   | Opens   | [PASS]  |         |         |
| TMTSG-6 |         | "Add    | up      | {.statu |         |         |
|         |         | New     | cosi    | s-macro |         |         |
|         |         | Cosig   | gnatory | .aui-   |         |         |
|         |         | natory" | public  | lozenge |         |         |
|         |         |         | key     | .aui-lo |         |         |
|         |         |         | field   | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| CV      |         | Input   | Shows a | [PASS]  |         |         |
| TMTSG-7 |         | invalid | message | {.statu |         |         |
|         |         | public  | "       | s-macro |         |         |
|         |         | key     | Invalid | .aui-   |         |         |
|         |         |         | Input"  | lozenge |         |         |
|         |         |         |         | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| CV      |         | Click   | Shows   | [PASS]  |         |         |
| TMTSG-8 |         | on      | all     | {.statu |         |         |
|         |         | "C      | normal  | s-macro |         |         |
|         |         | ontact" | a       | .aui-   |         |         |
|         |         | icon    | ccounts | lozenge |         |         |
|         |         |         | and     | .aui-lo |         |         |
|         |         |         | c       | zenge-s |         |         |
|         |         |         | ontacts | uccess} |         |         |
|         |         |         | av      |         |         |         |
|         |         |         | ailable |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| CV      | P       | Leave   | Shows a | [PASS]  |         |         |
| TMTSG-9 | assword | p       | message | {.statu |         |         |
|         |         | assword | "Wallet | s-macro |         |         |
|         |         | field   | p       | .aui-   |         |         |
|         |         | empty   | assword | lozenge |         |         |
|         |         |         | is      | .aui-lo |         |         |
|         |         |         | re      | zenge-s |         |         |
|         |         |         | quired" | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| CVT     | Clear   | Click   | User is | [PASS]  |         |         |
| MTSG-10 |         | "       | d       | {.statu |         |         |
|         |         | Cancel" | irected | s-macro |         |         |
|         |         |         | back to | .aui-   |         |         |
|         |         |         | m       | lozenge |         |         |
|         |         |         | ultisig | .aui-lo |         |         |
|         |         |         | s       | zenge-s |         |         |
|         |         |         | ettings | uccess} |         |         |
|         |         |         | page    |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| CVT     | Send    | Click   | C       | [PASS]  |         |         |
| MTSG-11 |         | "Update | onverts | {.statu |         |         |
|         |         | Cosigna | account | s-macro |         |         |
|         |         | tories" | to      | .aui-   |         |         |
|         |         | when    | m       | lozenge |         |         |
|         |         | there   | ultisig | .aui-lo |         |         |
|         |         | is at   |         | zenge-s |         |         |
|         |         | least   |         | uccess} |         |         |
|         |         | one     |         |         |         |         |
|         |         | cosi    |         |         |         |         |
|         |         | gnatory |         |         |         |         |
|         |         | added   |         |         |         |         |
|         |         | and     |         |         |         |         |
|         |         | p       |         |         |         |         |
|         |         | assword |         |         |         |         |
|         |         | field   |         |         |         |         |
|         |         | is      |         |         |         |         |
|         |         | filled  |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| CVT     |         | Click   | Shows a | [PASS]  |         |         |
| MTSG-12 |         | "Update | message | {.statu |         |         |
|         |         | Cosigna | "P      | s-macro |         |         |
|         |         | tories" | assword | .aui-   |         |         |
|         |         | when    | for     | lozenge |         |         |
|         |         | p       | wallet  | .aui-lo |         |         |
|         |         | assword | \<name  | zenge-s |         |         |
|         |         | is      | of      | uccess} |         |         |
|         |         | invalid | w       |         |         |         |
|         |         |         | allet\> |         |         |         |
|         |         |         | is      |         |         |         |
|         |         |         | i       |         |         |         |
|         |         |         | nvalid" |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ###     |         |         |         |         |         |         |
|  Edit M |         |         |         |         |         |         |
| ultisig |         |         |         |         |         |         |
|  {#Test |         |         |         |         |         |         |
| Report- |         |         |         |         |         |         |
| 1.1.8-1 |         |         |         |         |         |         |
| -EditMu |         |         |         |         |         |         |
| ltisig} |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ED      | Manage  | Click   | Edit    | [PASS]  |         |         |
| TMTSG-1 | Cosign  | manage  | M       | {.statu |         |         |
|         | atories | cosign  | ultisig | s-macro |         |         |
|         |         | atories | page is | .aui-   |         |         |
|         |         |         | di      | lozenge |         |         |
|         |         |         | splayed | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ED      | Remove  | Click   | Cosign  | [PASS]  |         |         |
| TMTSG-2 | cosi    | on drop | atories | {.statu |         |         |
|         | gnatory | down    | are     | s-macro |         |         |
|         |         | icon    | di      | .aui-   |         |         |
|         |         |         | splayed | lozenge |         |         |
|         |         |         |         | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ED      |         | Click   | S       | [PASS]  |         |         |
| TMTSG-3 |         | on      | elected | {.statu |         |         |
|         |         | delete  | c       | s-macro |         |         |
|         |         | icon    | osigner | .aui-   |         |         |
|         |         |         | is      | lozenge |         |         |
|         |         |         | high    | .aui-lo |         |         |
|         |         |         | lighted | zenge-s |         |         |
|         |         |         | as      | uccess} |         |         |
|         |         |         | r       |         |         |         |
|         |         |         | emoving |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ED      | Add     | Click   | Opens   | [PASS]  |         |         |
| TMTSG-4 | Cosi    | Add     | up      | {.statu |         |         |
|         | gnatory | Cosi    | cosi    | s-macro |         |         |
|         |         | gnatory | gnatory | .aui-   |         |         |
|         |         |         | public  | lozenge |         |         |
|         |         |         | key     | .aui-lo |         |         |
|         |         |         | field   | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ED      |         | Input   | Shows   | [PASS]  |         |         |
| TMTSG-5 |         | invalid | invalid | {.statu |         |         |
|         |         | public  | public  | s-macro |         |         |
|         |         | key     | key     | .aui-   |         |         |
|         |         |         | error   | lozenge |         |         |
|         |         |         |         | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ED      |         | Click   | Shows   | [PASS]  |         |         |
| TMTSG-6 |         | on      | all     | {.statu |         |         |
|         |         | contact | normal  | s-macro |         |         |
|         |         | icon    | a       | .aui-   |         |         |
|         |         |         | ccounts | lozenge |         |         |
|         |         |         | and     | .aui-lo |         |         |
|         |         |         | c       | zenge-s |         |         |
|         |         |         | ontacts | uccess} |         |         |
|         |         |         | av      |         |         |         |
|         |         |         | ailable |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ED      | Scheme  | Click   | M       | [PASS]  |         |         |
| TMTSG-7 |         | on      | ultisig | {.statu |         |         |
|         |         | scheme  | graph   | s-macro |         |         |
|         |         | section | scheme  | .aui-   |         |         |
|         |         |         | is      | lozenge |         |         |
|         |         |         | di      | .aui-lo |         |         |
|         |         |         | splayed | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ED      |         | Radio   | Scheme  | [PASS]  |         |         |
| TMTSG-8 |         | buttons | can be  | {.statu |         |         |
|         |         |         | seen    | s-macro |         |         |
|         |         |         | ve      | .aui-   |         |         |
|         |         |         | rtical, | lozenge |         |         |
|         |         |         | horiz   | .aui-lo |         |         |
|         |         |         | iontal, | zenge-s |         |         |
|         |         |         | right   | uccess} |         |         |
|         |         |         | to      |         |         |         |
|         |         |         | left,   |         |         |         |
|         |         |         | left to |         |         |         |
|         |         |         | right   |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ED      | Select  | Select  | D       | [PASS]  |         |         |
| TMTSG-9 | cosi    | main    | isplays | {.statu |         |         |
|         | gnatory | cosi    | all     | s-macro |         |         |
|         |         | gnatory | cosign  | .aui-   |         |         |
|         |         | d       | atories | lozenge |         |         |
|         |         | ropdown | av      | .aui-lo |         |         |
|         |         |         | ailable | zenge-s |         |         |
|         |         |         | in the  | uccess} |         |         |
|         |         |         | wallet  |         |         |         |
|         |         |         | except  |         |         |         |
|         |         |         | s       |         |         |         |
|         |         |         | elected |         |         |         |
|         |         |         | c       |         |         |         |
|         |         |         | osigner |         |         |         |
|         |         |         | from    |         |         |         |
|         |         |         | other   |         |         |         |
|         |         |         | cosi    |         |         |         |
|         |         |         | gnatory |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| EDT     |         | Select  | D       | [PASS]  |         |         |
| MTSG-10 |         | other   | isplays | {.statu |         |         |
|         |         | cosi    | all     | s-macro |         |         |
|         |         | gnatory | cosign  | .aui-   |         |         |
|         |         | d       | atories | lozenge |         |         |
|         |         | ropdown | av      | .aui-lo |         |         |
|         |         |         | ailable | zenge-s |         |         |
|         |         |         | in the  | uccess} |         |         |
|         |         |         | wallet  |         |         |         |
|         |         |         | except  |         |         |         |
|         |         |         | s       |         |         |         |
|         |         |         | elected |         |         |         |
|         |         |         | c       |         |         |         |
|         |         |         | osigner |         |         |         |
|         |         |         | from    |         |         |         |
|         |         |         | main    |         |         |         |
|         |         |         | cosi    |         |         |         |
|         |         |         | gnatory |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| EDT     | P       | Leave   | D       | [PASS]  |         |         |
| MTSG-11 | assword | p       | isplays | {.statu |         |         |
|         |         | assword | p       | s-macro |         |         |
|         |         | field   | assword | .aui-   |         |         |
|         |         | empty   | is      | lozenge |         |         |
|         |         |         | r       | .aui-lo |         |         |
|         |         |         | equired | zenge-s |         |         |
|         |         |         | error   | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| EDT     | Update  | Click   | Edit    | [PASS]  |         |         |
| MTSG-12 | Cosign  | update  | m       | {.statu |         |         |
|         | atories | cosign  | ultisig | s-macro |         |         |
|         |         | atories | account | .aui-   |         |         |
|         |         | when    |         | lozenge |         |         |
|         |         | p       |         | .aui-lo |         |         |
|         |         | assword |         | zenge-s |         |         |
|         |         | field   |         | uccess} |         |         |
|         |         | is      |         |         |         |         |
|         |         | filled  |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| EDT     |         | Click   | Send    | [PASS]  |         |         |
| MTSG-13 |         | update  | button  | {.statu |         |         |
|         |         | cosign  | is      | s-macro |         |         |
|         |         | atories | d       | .aui-   |         |         |
|         |         | when    | isabled | lozenge |         |         |
|         |         | scheme  | and     | .aui-lo |         |         |
|         |         | transa  | error   | zenge-s |         |         |
|         |         | ctional | message | uccess} |         |         |
|         |         | values  | will be |         |         |         |
|         |         | are     | shown   |         |         |         |
|         |         | a       |         |         |         |         |
|         |         | djusted |         |         |         |         |
|         |         | to 0    |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| EDT     |         | Click   | Send    | [PASS]  |         |         |
| MTSG-14 |         | update  | button  | {.statu |         |         |
|         |         | cosign  | is      | s-macro |         |         |
|         |         | atories | d       | .aui-   |         |         |
|         |         | when    | isabled | lozenge |         |         |
|         |         | scheme  | and     | .aui-lo |         |         |
|         |         | account | error   | zenge-s |         |         |
|         |         | d       | message | uccess} |         |         |
|         |         | eletion | will be |         |         |         |
|         |         | values  | shown   |         |         |         |
|         |         | are     |         |         |         |         |
|         |         | a       |         |         |         |         |
|         |         | djusted |         |         |         |         |
|         |         | to 0    |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| EDT     |         | Click   | D       | [PASS]  |         |         |
| MTSG-15 |         | send    | isplays | {.statu |         |         |
|         |         | when    | p       | s-macro |         |         |
|         |         | p       | assword | .aui-   |         |         |
|         |         | assword | invalid | lozenge |         |         |
|         |         | is      | error   | .aui-lo |         |         |
|         |         | invalid |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
:::

::: table-wrap
+-----------+-----------+-----------+-----------+-----------+---+---+
| ### Out   |           |           |           |           |   |   |
| going Swa |           |           |           |           |   |   |
| p {#TestR |           |           |           |           |   |   |
| eport-1.1 |           |           |           |           |   |   |
| .8-1-Outg |           |           |           |           |   |   |
| oingSwap} |           |           |           |           |   |   |
+-----------+-----------+-----------+-----------+-----------+---+---+
| OUTSWAP-1 | Swap      | Click     | Main      | [P        |   |   |
|           |           | swap      | network   | ASS]{.sta |   |   |
|           |           | under     | swap page | tus-macro |   |   |
|           |           | Quick     | is        | .au       |   |   |
|           |           | Action    | displayed | i-lozenge |   |   |
|           |           |           |           | .au       |   |   |
|           |           |           |           | i-lozenge |   |   |
|           |           |           |           | -success} |   |   |
+-----------+-----------+-----------+-----------+-----------+---+---+
| OUTSWAP-2 |           | Click     | Main      | [P        |   |   |
|           |           | swap on   | network   | ASS]{.sta |   |   |
|           |           | the       | swap page | tus-macro |   |   |
|           |           | dashboard | is        | .au       |   |   |
|           |           |           | displayed | i-lozenge |   |   |
|           |           |           |           | .au       |   |   |
|           |           |           |           | i-lozenge |   |   |
|           |           |           |           | -success} |   |   |
+-----------+-----------+-----------+-----------+-----------+---+---+
| OUTSWAP-3 | Outgoing  | Click     | Outgoing  | [P        |   |   |
|           | swap      | dropdown  | swap      | ASS]{.sta |   |   |
|           |           | list \>   | tr        | tus-macro |   |   |
|           |           |           | ansaction | .au       |   |   |
|           |           | select    | details   | i-lozenge |   |   |
|           |           | sirius    | page is   | .au       |   |   |
|           |           | chain to  | displayed | i-lozenge |   |   |
|           |           | bsc       |           | -success} |   |   |
+-----------+-----------+-----------+-----------+-----------+---+---+
| OUTSWAP-4 | Select    | Click on  | Displays  | [P        |   |   |
|           | asset     | select    | asset     | ASS]{.sta |   |   |
|           |           | asset     | available | tus-macro |   |   |
|           |           | dropdown  | for       | .au       |   |   |
|           |           | list      | tr        | i-lozenge |   |   |
|           |           |           | ansaction | .au       |   |   |
|           |           |           |           | i-lozenge |   |   |
|           |           |           |           | -success} |   |   |
+-----------+-----------+-----------+-----------+-----------+---+---+
| OUTSWAP-5 | Select    | Click on  | Available | [P        |   |   |
|           | Account   | tr        | account   | ASS]{.sta |   |   |
|           |           | ansaction | dropdown  | tus-macro |   |   |
|           |           | details   | list will | .au       |   |   |
|           |           | dropdown  | show up,  | i-lozenge |   |   |
|           |           | list      | user can  | .au       |   |   |
|           |           |           | select    | i-lozenge |   |   |
|           |           |           | which     | -success} |   |   |
|           |           |           | account   |           |   |   |
|           |           |           | to be     |           |   |   |
|           |           |           | chosen    |           |   |   |
|           |           |           | for       |           |   |   |
|           |           |           | tr        |           |   |   |
|           |           |           | ansaction |           |   |   |
+-----------+-----------+-----------+-----------+-----------+---+---+
| OUTSWAP-6 | Transfer  | Leave     | Prompt    | [P        |   |   |
|           | Amount    | transfer  | error     | ASS]{.sta |   |   |
|           |           | amount as | message   | tus-macro |   |   |
|           |           | 0         | "Amount   | .au       |   |   |
|           |           |           | is Empty" | i-lozenge |   |   |
|           |           |           |           | .au       |   |   |
|           |           |           |           | i-lozenge |   |   |
|           |           |           |           | -success} |   |   |
+-----------+-----------+-----------+-----------+-----------+---+---+
| OUTSWAP-7 |           | Amount    | Prompt    | [P        |   |   |
|           |           | exceeding | error     | ASS]{.sta |   |   |
|           |           | account   | message   | tus-macro |   |   |
|           |           | balance   | "Ins      | .au       |   |   |
|           |           |           | ufficient | i-lozenge |   |   |
|           |           |           | balance"  | .au       |   |   |
|           |           |           |           | i-lozenge |   |   |
|           |           |           |           | -success} |   |   |
+-----------+-----------+-----------+-----------+-----------+---+---+
| OUTSWAP-8 |           | Account   | Prompt    | [P        |   |   |
|           |           | balance   | error     | ASS]{.sta |   |   |
|           |           | less than | message   | tus-macro |   |   |
|           |           | tr        | "Balance  | .au       |   |   |
|           |           | ansaction | is        | i-lozenge |   |   |
|           |           | fee       | ins       | .au       |   |   |
|           |           |           | ufficient | i-lozenge |   |   |
|           |           |           | to cover  | -success} |   |   |
|           |           |           | tr        |           |   |   |
|           |           |           | ansaction |           |   |   |
|           |           |           | fee" and  |           |   |   |
|           |           |           | transfer  |           |   |   |
|           |           |           | button is |           |   |   |
|           |           |           | disabled  |           |   |   |
+-----------+-----------+-----------+-----------+-----------+---+---+
| OUTSWAP-9 | Metamask  | Leave     | Shows a   | [P        |   |   |
|           | address   | metamask  | error     | ASS]{.sta |   |   |
|           |           | address   | message   | tus-macro |   |   |
|           |           | empty     | "Valid    | .au       |   |   |
|           |           |           | BSC       | i-lozenge |   |   |
|           |           |           | address   | .au       |   |   |
|           |           |           | is        | i-lozenge |   |   |
|           |           |           | required" | -success} |   |   |
+-----------+-----------+-----------+-----------+-----------+---+---+
| O         | Tr        | Select on | tr        | [P        |   |   |
| UTSWAP-10 | ansaction | tr        | ansaction | ASS]{.sta |   |   |
|           | fee       | ansaction | fee type  | tus-macro |   |   |
|           |           | fee type  | will be   | .au       |   |   |
|           |           |           | selected  | i-lozenge |   |   |
|           |           |           |           | .au       |   |   |
|           |           |           |           | i-lozenge |   |   |
|           |           |           |           | -success} |   |   |
+-----------+-----------+-----------+-----------+-----------+---+---+
| O         |           | Tr        | Tr        | [P        |   |   |
| UTSWAP-11 |           | ansaction | ansaction | ASS]{.sta |   |   |
|           |           | fee       | fee will  | tus-macro |   |   |
|           |           | ca        | be        | .au       |   |   |
|           |           | lculation | c         | i-lozenge |   |   |
|           |           |           | alculated | .au       |   |   |
|           |           |           | directly  | i-lozenge |   |   |
|           |           |           | into      | -success} |   |   |
|           |           |           | total     |           |   |   |
|           |           |           | tr        |           |   |   |
|           |           |           | ansaction |           |   |   |
|           |           |           | fee       |           |   |   |
+-----------+-----------+-----------+-----------+-----------+---+---+
| O         | Password  | Leave the | Shows a   | [P        |   |   |
| UTSWAP-12 |           | password  | error     | ASS]{.sta |   |   |
|           |           | field as  | message   | tus-macro |   |   |
|           |           | empty or  | "Password | .au       |   |   |
|           |           | less than | is        | i-lozenge |   |   |
|           |           | required  | required" | .au       |   |   |
|           |           | values    |           | i-lozenge |   |   |
|           |           |           |           | -success} |   |   |
+-----------+-----------+-----------+-----------+-----------+---+---+
| O         | Outgoing  | Enter     | Swap      | [P        |   |   |
| UTSWAP-13 | swap      | valid     | tr        | ASS]{.sta |   |   |
|           | tr        | wallet    | ansaction | tus-macro |   |   |
|           | ansaction | address,  | will be   | .au       |   |   |
|           | (xpx)     | valid     | suc       | i-lozenge |   |   |
|           |           | transfer  | cessfully | .au       |   |   |
|           |           | amount    | created,  | i-lozenge |   |   |
|           |           | and       | not       | -success} |   |   |
|           |           | correct   | ification |           |   |   |
|           |           | wallet    | prompted  |           |   |   |
|           |           | password, | and user  |           |   |   |
|           |           | click     | directed  |           |   |   |
|           |           | transfer  | to        |           |   |   |
|           |           |           | s         |           |   |   |
|           |           |           | uccessful |           |   |   |
|           |           |           | swap      |           |   |   |
|           |           |           | details   |           |   |   |
|           |           |           | page      |           |   |   |
+-----------+-----------+-----------+-----------+-----------+---+---+
| O         |           | Enter     | Swap      | [P        |   |   |
| UTSWAP-14 |           | valid     | tr        | ASS]{.sta |   |   |
|           |           | wallet    | ansaction | tus-macro |   |   |
|           |           | address,  | failed    | .au       |   |   |
|           |           | valid     | with      | i-lozenge |   |   |
|           |           | transfer  | error     | .au       |   |   |
|           |           | amount    | message   | i-lozenge |   |   |
|           |           | and       | shown     | -success} |   |   |
|           |           | incorrect | "Password |           |   |   |
|           |           | wallet    | for       |           |   |   |
|           |           | password, | wallet    |           |   |   |
|           |           | click     | \<wallet  |           |   |   |
|           |           | transfer  | name\> is |           |   |   |
|           |           |           | invalid"  |           |   |   |
+-----------+-----------+-----------+-----------+-----------+---+---+
| O         | Outgoing  | Enter     | Swap      | [P        |   |   |
| UTSWAP-15 | swap      | valid     | tr        | ASS]{.sta |   |   |
|           | tr        | wallet    | ansaction | tus-macro |   |   |
|           | ansaction | address,  | will be   | .au       |   |   |
|           | (metX)    | valid     | suc       | i-lozenge |   |   |
|           |           | transfer  | cessfully | .au       |   |   |
|           |           | amount    | created,  | i-lozenge |   |   |
|           |           | and       | not       | -success} |   |   |
|           |           | correct   | ification |           |   |   |
|           |           | wallet    | prompted  |           |   |   |
|           |           | password, | and user  |           |   |   |
|           |           | click     | directed  |           |   |   |
|           |           | transfer  | to        |           |   |   |
|           |           |           | s         |           |   |   |
|           |           |           | uccessful |           |   |   |
|           |           |           | swap      |           |   |   |
|           |           |           | details   |           |   |   |
|           |           |           | page      |           |   |   |
+-----------+-----------+-----------+-----------+-----------+---+---+
| O         |           | Enter     | Swap      | [P        |   |   |
| UTSWAP-16 |           | valid     | tr        | ASS]{.sta |   |   |
|           |           | wallet    | ansaction | tus-macro |   |   |
|           |           | address,  | failed    | .au       |   |   |
|           |           | valid     | with      | i-lozenge |   |   |
|           |           | transfer  | error     | .au       |   |   |
|           |           | amount    | message   | i-lozenge |   |   |
|           |           | and       | shown     | -success} |   |   |
|           |           | incorrect | "Password |           |   |   |
|           |           | wallet    | for       |           |   |   |
|           |           | password, | wallet    |           |   |   |
|           |           | click     | \<wallet  |           |   |   |
|           |           | transfer  | name\> is |           |   |   |
|           |           |           | invalid"  |           |   |   |
+-----------+-----------+-----------+-----------+-----------+---+---+
| O         | Cancel    | Click on  | Swap      | [P        |   |   |
| UTSWAP-17 |           | "Later"   | tr        | ASS]{.sta |   |   |
|           |           | icon      | ansaction | tus-macro |   |   |
|           |           | button    | c         | .au       |   |   |
|           |           |           | ancelled, | i-lozenge |   |   |
|           |           |           | user      | .au       |   |   |
|           |           |           | directed  | i-lozenge |   |   |
|           |           |           | back to   | -success} |   |   |
|           |           |           | main      |           |   |   |
|           |           |           | network   |           |   |   |
|           |           |           | swap page |           |   |   |
+-----------+-----------+-----------+-----------+-----------+---+---+
| O         | Eye icon  | Click on  | Show/hide | [P        |   |   |
| UTSWAP-17 |           | eye icon  | password  | ASS]{.sta |   |   |
|           |           | button    |           | tus-macro |   |   |
|           |           |           |           | .au       |   |   |
|           |           |           |           | i-lozenge |   |   |
|           |           |           |           | .au       |   |   |
|           |           |           |           | i-lozenge |   |   |
|           |           |           |           | -success} |   |   |
+-----------+-----------+-----------+-----------+-----------+---+---+
:::

::: table-wrap
+-----------+-----------+-----------+-----------+-----------+---+---+
| *         |           |           |           |           |   |   |
| *Incoming |           |           |           |           |   |   |
| Swap**    |           |           |           |           |   |   |
+-----------+-----------+-----------+-----------+-----------+---+---+
| INSWAP-1  | Swap      | Click     | Main      | [P        |   |   |
|           |           | swap      | network   | ASS]{.sta |   |   |
|           |           | under     | swap page | tus-macro |   |   |
|           |           | Quick     | is        | .au       |   |   |
|           |           | Action    | displayed | i-lozenge |   |   |
|           |           |           |           | .au       |   |   |
|           |           |           |           | i-lozenge |   |   |
|           |           |           |           | -success} |   |   |
+-----------+-----------+-----------+-----------+-----------+---+---+
| INSWAP-2  |           | Click     | Main      | [P        |   |   |
|           |           | swap on   | network   | ASS]{.sta |   |   |
|           |           | the       | swap page | tus-macro |   |   |
|           |           | dashboard | is        | .au       |   |   |
|           |           |           | displayed | i-lozenge |   |   |
|           |           |           |           | .au       |   |   |
|           |           |           |           | i-lozenge |   |   |
|           |           |           |           | -success} |   |   |
+-----------+-----------+-----------+-----------+-----------+---+---+
| INSWAP-3  | Incoming  | Click     | Incoming  | [P        |   |   |
|           | swap      | dropdown  | swap      | ASS]{.sta |   |   |
|           |           | list \>   | tr        | tus-macro |   |   |
|           |           |           | ansaction | .au       |   |   |
|           |           | select    | details   | i-lozenge |   |   |
|           |           | bsc to    | page is   | .au       |   |   |
|           |           | sirius    | displayed | i-lozenge |   |   |
|           |           | chain     |           | -success} |   |   |
+-----------+-----------+-----------+-----------+-----------+---+---+
| INSWAP-4  | Select    | Click on  | Displays  | [P        |   |   |
|           | asset     | select    | asset     | ASS]{.sta |   |   |
|           |           | asset     | available | tus-macro |   |   |
|           |           | dropdown  | for       | .au       |   |   |
|           |           | list      | tr        | i-lozenge |   |   |
|           |           |           | ansaction | .au       |   |   |
|           |           |           |           | i-lozenge |   |   |
|           |           |           |           | -success} |   |   |
+-----------+-----------+-----------+-----------+-----------+---+---+
| INSWAP-5  | Select    | Click on  | Available | [P        |   |   |
|           | Account   | tr        | account   | ASS]{.sta |   |   |
|           |           | ansaction | dropdown  | tus-macro |   |   |
|           |           | details   | list will | .au       |   |   |
|           |           | dropdown  | show up,  | i-lozenge |   |   |
|           |           | list      | user can  | .au       |   |   |
|           |           |           | select    | i-lozenge |   |   |
|           |           |           | which     | -success} |   |   |
|           |           |           | account   |           |   |   |
|           |           |           | to be     |           |   |   |
|           |           |           | chosen    |           |   |   |
|           |           |           | for       |           |   |   |
|           |           |           | tr        |           |   |   |
|           |           |           | ansaction |           |   |   |
+-----------+-----------+-----------+-----------+-----------+---+---+
| INSWAP-6  | Transfer  | Leave     | Prompt    | [P        |   |   |
|           | Amount    | transfer  | error     | ASS]{.sta |   |   |
|           |           | amount as | message   | tus-macro |   |   |
|           |           | 0         | "Minimum  | .au       |   |   |
|           |           |           | amount is | i-lozenge |   |   |
|           |           |           | 51"       | .au       |   |   |
|           |           |           |           | i-lozenge |   |   |
|           |           |           |           | -success} |   |   |
+-----------+-----------+-----------+-----------+-----------+---+---+
| INSWAP-7  |           | Amount    | Prompt    | [P        |   |   |
|           |           | exceeding | error     | ASS]{.sta |   |   |
|           |           | account   | message   | tus-macro |   |   |
|           |           | balance   | "Ins      | .au       |   |   |
|           |           |           | ufficient | i-lozenge |   |   |
|           |           |           | token     | .au       |   |   |
|           |           |           | balance"  | i-lozenge |   |   |
|           |           |           |           | -success} |   |   |
+-----------+-----------+-----------+-----------+-----------+---+---+
| INSWAP-8  |           | Valid     | Error     | [P        |   |   |
|           |           | transfer  | message   | ASS]{.sta |   |   |
|           |           | amount    | will      | tus-macro |   |   |
|           |           |           | disappear | .au       |   |   |
|           |           |           | and "send | i-lozenge |   |   |
|           |           |           | request"  | .au       |   |   |
|           |           |           | button    | i-lozenge |   |   |
|           |           |           | will be   | -success} |   |   |
|           |           |           | enabled   |           |   |   |
+-----------+-----------+-----------+-----------+-----------+---+---+
| INSWAP-10 | Sirius    | Click on  | Shows a   | [P        |   |   |
|           | chain     | Sirius    | dropdown  | ASS]{.sta |   |   |
|           | account   | chain     | list of   | tus-macro |   |   |
|           |           | account   | available | .au       |   |   |
|           |           | dropdown  | account   | i-lozenge |   |   |
|           |           | list      | within    | .au       |   |   |
|           |           |           | the       | i-lozenge |   |   |
|           |           |           | wallet    | -success} |   |   |
+-----------+-----------+-----------+-----------+-----------+---+---+
| INSWAP-11 | Total     | Total     | Transfer  | [P        |   |   |
|           | transfer  | transfer  | amount    | ASS]{.sta |   |   |
|           | amount    | amount    | will be   | tus-macro |   |   |
|           |           | shown     | shown     | .au       |   |   |
|           |           |           | after     | i-lozenge |   |   |
|           |           |           |           | .au       |   |   |
|           |           |           |           | i-lozenge |   |   |
|           |           |           |           | -success} |   |   |
+-----------+-----------+-----------+-----------+-----------+---+---+
| INSWAP-12 | Send      | Click on  | Request   | [P        |   |   |
|           | request   | send      | for token | ASS]{.sta |   |   |
|           |           | request   | transfer  | tus-macro |   |   |
|           |           | button    | to sirius | .au       |   |   |
|           |           |           | will be   | i-lozenge |   |   |
|           |           |           | sent to   | .au       |   |   |
|           |           |           | selected  | i-lozenge |   |   |
|           |           |           | metamask  | -success} |   |   |
|           |           |           | address   |           |   |   |
+-----------+-----------+-----------+-----------+-----------+---+---+
| INSWAP-13 | Transfer  | Click on  | After     | [P        |   |   |
|           | V         | check     | getting   | ASS]{.sta |   |   |
|           | alidation | tr        | con       | tus-macro |   |   |
|           | (xpx)     | ansaction | firmation | .au       |   |   |
|           |           | con       | to        | i-lozenge |   |   |
|           |           | firmation | proceed   | .au       |   |   |
|           |           | to        | from      | i-lozenge |   |   |
|           |           | proceed   | metamask  | -success} |   |   |
|           |           |           | account,  |           |   |   |
|           |           |           | check     |           |   |   |
|           |           |           | tr        |           |   |   |
|           |           |           | ansaction |           |   |   |
|           |           |           | con       |           |   |   |
|           |           |           | firmation |           |   |   |
|           |           |           | to        |           |   |   |
|           |           |           | proceed   |           |   |   |
|           |           |           | button    |           |   |   |
|           |           |           | will be   |           |   |   |
|           |           |           | enabled   |           |   |   |
|           |           |           | and       |           |   |   |
|           |           |           | message   |           |   |   |
|           |           |           | will be   |           |   |   |
|           |           |           | sent to   |           |   |   |
|           |           |           | Metamask  |           |   |   |
+-----------+-----------+-----------+-----------+-----------+---+---+
| INSWAP-14 |           | Click on  | After     | [P        |   |   |
|           |           | continue  | getting   | ASS]{.sta |   |   |
|           |           |           | metamask  | tus-macro |   |   |
|           |           |           | account   | .au       |   |   |
|           |           |           | signature | i-lozenge |   |   |
|           |           |           | to        | .au       |   |   |
|           |           |           | proceed,  | i-lozenge |   |   |
|           |           |           | swap      | -success} |   |   |
|           |           |           | process   |           |   |   |
|           |           |           | completed |           |   |   |
|           |           |           | and user  |           |   |   |
|           |           |           | will be   |           |   |   |
|           |           |           | directed  |           |   |   |
|           |           |           | to        |           |   |   |
|           |           |           | s         |           |   |   |
|           |           |           | uccessful |           |   |   |
|           |           |           | swap      |           |   |   |
|           |           |           | details   |           |   |   |
|           |           |           | page      |           |   |   |
+-----------+-----------+-----------+-----------+-----------+---+---+
| INSWAP-15 | Transfer  | Click on  | After     | [P        |   |   |
|           | V         | check     | getting   | ASS]{.sta |   |   |
|           | alidation | tr        | con       | tus-macro |   |   |
|           | (metx)    | ansaction | firmation | .au       |   |   |
|           |           | con       | to        | i-lozenge |   |   |
|           |           | firmation | proceed   | .au       |   |   |
|           |           | to        | from      | i-lozenge |   |   |
|           |           | proceed   | metamask  | -success} |   |   |
|           |           |           | account,  |           |   |   |
|           |           |           | check     |           |   |   |
|           |           |           | tr        |           |   |   |
|           |           |           | ansaction |           |   |   |
|           |           |           | con       |           |   |   |
|           |           |           | firmation |           |   |   |
|           |           |           | to        |           |   |   |
|           |           |           | proceed   |           |   |   |
|           |           |           | button    |           |   |   |
|           |           |           | will be   |           |   |   |
|           |           |           | enabled   |           |   |   |
|           |           |           | and       |           |   |   |
|           |           |           | message   |           |   |   |
|           |           |           | will be   |           |   |   |
|           |           |           | sent to   |           |   |   |
|           |           |           | metamask  |           |   |   |
+-----------+-----------+-----------+-----------+-----------+---+---+
| INSWAP-16 |           | Click on  | After     | [P        |   |   |
|           |           | continue  | getting   | ASS]{.sta |   |   |
|           |           |           | metamask  | tus-macro |   |   |
|           |           |           | account   | .au       |   |   |
|           |           |           | signature | i-lozenge |   |   |
|           |           |           | to        | .au       |   |   |
|           |           |           | proceed,  | i-lozenge |   |   |
|           |           |           | swap      | -success} |   |   |
|           |           |           | process   |           |   |   |
|           |           |           | completed |           |   |   |
|           |           |           | and user  |           |   |   |
|           |           |           | will be   |           |   |   |
|           |           |           | directed  |           |   |   |
|           |           |           | to        |           |   |   |
|           |           |           | s         |           |   |   |
|           |           |           | uccessful |           |   |   |
|           |           |           | swap      |           |   |   |
|           |           |           | details   |           |   |   |
|           |           |           | page      |           |   |   |
+-----------+-----------+-----------+-----------+-----------+---+---+
:::

## Services {#TestReport-1.1.8-1-Services}

### Namespaces {#TestReport-1.1.8-1-Namespaces}

#### Register {#TestReport-1.1.8-1-Register style="margin-left: 30.0px;"}

#### Extend Duration {#TestReport-1.1.8-1-ExtendDuration style="margin-left: 30.0px;"}

### Assets {#TestReport-1.1.8-1-Assets}

#### Create {#TestReport-1.1.8-1-Create style="margin-left: 30.0px;"}

#### Modify Supply {#TestReport-1.1.8-1-ModifySupply style="margin-left: 30.0px;"}

#### Link to Namespaces {#TestReport-1.1.8-1-LinktoNamespaces style="margin-left: 30.0px;"}

### Swap {#TestReport-1.1.8-1-Swap}

#### NIS1 {#TestReport-1.1.8-1-NIS1 style="margin-left: 30.0px;"}

#### ETH {#TestReport-1.1.8-1-ETH style="margin-left: 30.0px;"}

#### BSC {#TestReport-1.1.8-1-BSC style="margin-left: 30.0px;"}

### Address Book {#TestReport-1.1.8-1-AddressBook}

#### List {#TestReport-1.1.8-1-List style="margin-left: 30.0px;"}

#### Add Contacts {#TestReport-1.1.8-1-AddContacts style="margin-left: 30.0px;"}

### Wallets {#TestReport-1.1.8-1-Wallets}

#### Change Password {#TestReport-1.1.8-1-ChangePassword style="margin-left: 30.0px;"}

#### Export {#TestReport-1.1.8-1-Export style="margin-left: 30.0px;"}

#### Delete {#TestReport-1.1.8-1-Delete style="margin-left: 30.0px;"}

### Voting {#TestReport-1.1.8-1-Voting}

#### Create Poll {#TestReport-1.1.8-1-CreatePoll style="margin-left: 30.0px;"}

#### Vote {#TestReport-1.1.8-1-Vote style="margin-left: 30.0px;"}

#### View Results {#TestReport-1.1.8-1-ViewResults style="margin-left: 30.0px;"}

### Storage {#TestReport-1.1.8-1-Storage}

#### Files {#TestReport-1.1.8-1-Files style="margin-left: 30.0px;"}

#### Upload File {#TestReport-1.1.8-1-UploadFile style="margin-left: 30.0px;"}

#### Send/Share {#TestReport-1.1.8-1-Send/Share style="margin-left: 30.0px;"}

### Sirius Gift {#TestReport-1.1.8-1-SiriusGift}

#### Create {#TestReport-1.1.8-1-Create.1 style="margin-left: 30.0px;"}

#### Redeem {#TestReport-1.1.8-1-Redeem style="margin-left: 30.0px;"}

### Aggregate Transactions {#TestReport-1.1.8-1-AggregateTransactions}

#### Complete {#TestReport-1.1.8-1-Complete style="margin-left: 30.0px;"}

#### Bonded {#TestReport-1.1.8-1-Bonded style="margin-left: 30.0px;"}
:::

::: {.pageSection .group}
::: pageSectionHeader
## Attachments: {#attachments .pageSectionTitle}
:::

::: {.greybox align="left"}
![](images/icons/bullet_blue.gif){height="8" width="8"}
[image-20220321-033506.png](attachments/2499248129/2499248143.png)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[image-20220321-013652.png](attachments/2499248129/2499248146.png)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[JuJFRQviEuNr-LFhKKtzgok1mpF5HDikOIL1_xWg6aGr2qkQ8QSbxpffBmBBZjHP0mp8bWeQOwXRWRwlDCdz6gs25qus8boYnGvW4GVGSyi0cdVFcdwMCJyRp_oVci2AbNXYamEotatFLomrkg](attachments/2499248129/2499248149)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[-bO8lWnCxvS5X986IxWgckBxaJCAbxhYl3-TF3royi6Q4j9TP6fotHOWiQ-il3_ryQNouMJ4csO5ZSgD_ZjKbkejc_edkj4PbVtm6f83nPyVS5LMbxvR1CSNaPwQrwZqw6pPpu1WRhThCx6m3A](attachments/2499248129/2499248152)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[b6Y7vdCjGYj4Iz0F_WS65i2cmIOlSUT86qa6i_8b-nI5nMCdfPd8pzyZ7F00oJUCaExJm6trTRKlkKGVJ7Sk77IHaRM8J3xiPRDc7QBvZKdGSgTdYDf5PENJN1AGkDy16cx3ElRHYzDKpmmMJA](attachments/2499248129/2499248155)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2499248129/2499248158)
(image/png)\
:::
:::
:::
:::

::: {#footer role="contentinfo"}
::: {.section .footer-body}
Document generated by Confluence on Nov 02, 2022 14:20

::: {#footer-logo}
[Atlassian](http://www.atlassian.com/)
:::
:::
:::
:::
