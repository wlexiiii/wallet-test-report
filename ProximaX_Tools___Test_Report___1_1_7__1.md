::: {#page}
::: {#main .aui-page-panel}
::: {#main-header}
::: {#breadcrumb-section}
1.  [ProximaX Tools](index.html)
2.  [Test Reports](Test-Reports_2443871313.html)
:::

# [ ProximaX Tools : Test Report - 1.1.7 -1 ]{#title-text} {#title-heading .pagetitle}
:::

::: {#content .view}
::: page-metadata
Created by [ davidwunarsa]{.author}, last modified on Jun 21, 2022
:::

::: {#main-content .wiki-content .group}
Date: 27/05/2022 - 27/05/2022\
Version: 1.1.7-1\
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

::: {.toc-macro .rbtoc1667369999384}
-   [Main Page](#TestReport-1.1.7-1-MainPage)
    -   [Sign In](#TestReport-1.1.7-1-SignIn)
    -   [Create New Wallet](#TestReport-1.1.7-1-CreateNewWallet)
    -   [Create New Wallet From Private
        Key](#TestReport-1.1.7-1-CreateNewWalletFromPrivateKey)
    -   [Import wallet from .wlt file (Create Wallet from a Wallet
        Backup)](#TestReport-1.1.7-1-Importwalletfrom.wltfile(CreateWalletfromaWalletBackup))
-   [Dashboard](#TestReport-1.1.7-1-Dashboard)
-   [Side Menu Bar (Home
    Page)](#TestReport-1.1.7-1-SideMenuBar(HomePage))
-   [Transfer (New Design)](#TestReport-1.1.7-1-Transfer(NewDesign))
-   [Accounts](#TestReport-1.1.7-1-Accounts)
    -   [Select Creation Type](#TestReport-1.1.7-1-SelectCreationType)
        -   [Create a New Account in the same
            Wallet](#TestReport-1.1.7-1-CreateaNewAccountinthesameWallet)
        -   [Create a New Account from Private Key in the same
            Wallet](#TestReport-1.1.7-1-CreateaNewAccountfromPrivateKeyinthesameWallet)
    -   [Edit an existing
        Account](#TestReport-1.1.7-1-EditanexistingAccount)
        -   [Details](#TestReport-1.1.7-1-Details)
    -   [Convert to Multisig](#TestReport-1.1.7-1-ConverttoMultisig)
    -   [Edit Multisig](#TestReport-1.1.7-1-EditMultisig)
    -   [Outgoing Swap](#TestReport-1.1.7-1-OutgoingSwap)
-   [Services](#TestReport-1.1.7-1-Services)
    -   [Namespaces](#TestReport-1.1.7-1-Namespaces)
        -   [Register](#TestReport-1.1.7-1-Register)
        -   [Extend Duration](#TestReport-1.1.7-1-ExtendDuration)
    -   [Assets](#TestReport-1.1.7-1-Assets)
        -   [Create](#TestReport-1.1.7-1-Create)
        -   [Modify Supply](#TestReport-1.1.7-1-ModifySupply)
        -   [Link to Namespaces](#TestReport-1.1.7-1-LinktoNamespaces)
    -   [Swap](#TestReport-1.1.7-1-Swap)
        -   [NIS1](#TestReport-1.1.7-1-NIS1)
        -   [ETH](#TestReport-1.1.7-1-ETH)
        -   [BSC](#TestReport-1.1.7-1-BSC)
    -   [Address Book](#TestReport-1.1.7-1-AddressBook)
        -   [List](#TestReport-1.1.7-1-List)
        -   [Add Contacts](#TestReport-1.1.7-1-AddContacts)
    -   [Wallets](#TestReport-1.1.7-1-Wallets)
        -   [Change Password](#TestReport-1.1.7-1-ChangePassword)
        -   [Export](#TestReport-1.1.7-1-Export)
        -   [Delete](#TestReport-1.1.7-1-Delete)
    -   [Voting](#TestReport-1.1.7-1-Voting)
        -   [Create Poll](#TestReport-1.1.7-1-CreatePoll)
        -   [Vote](#TestReport-1.1.7-1-Vote)
        -   [View Results](#TestReport-1.1.7-1-ViewResults)
    -   [Storage](#TestReport-1.1.7-1-Storage)
        -   [Files](#TestReport-1.1.7-1-Files)
        -   [Upload File](#TestReport-1.1.7-1-UploadFile)
        -   [Send/Share](#TestReport-1.1.7-1-Send/Share)
    -   [Sirius Gift](#TestReport-1.1.7-1-SiriusGift)
        -   [Create](#TestReport-1.1.7-1-Create.1)
        -   [Redeem](#TestReport-1.1.7-1-Redeem)
    -   [Aggregate
        Transactions](#TestReport-1.1.7-1-AggregateTransactions)
        -   [Complete](#TestReport-1.1.7-1-Complete)
        -   [Bonded](#TestReport-1.1.7-1-Bonded)
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
| .7-1-Ma |         |         |         |         |         |         |
| inPage} |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| **Test  | **Test  | **Test  | **E     | **S     | **R     | **Auto  |
| Case    | Scen    | steps** | xpected | tatus** | emark** | mated** |
| ID**    | arios** |         | r       |         |         |         |
|         |         |         | esult** |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| Main-1  | Sign in | Select  | Unable  | [PASS]  |         |         |
|         |         | wallet  | to sign | {.statu |         |         |
|         |         | and     | in,     | s-macro |         |         |
|         |         | click   | "Sign   | .aui-   |         |         |
|         |         | on      | In"     | lozenge |         |         |
|         |         | "Sign   | button  | .aui-lo |         |         |
|         |         | in"     | is      | zenge-s |         |         |
|         |         | button  | d       | uccess} |         |         |
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
| Main-2  | Sign in | Select  | Go to   | [PASS]  |         |         |
|         |         | wallet, | the     | {.statu |         |         |
|         |         | enter   | main    | s-macro |         |         |
|         |         | p       | home    | .aui-   |         |         |
|         |         | assword | page of | lozenge |         |         |
|         |         | and     | Sirius  | .aui-lo |         |         |
|         |         | click   | Wallet  | zenge-s |         |         |
|         |         | on      |         | uccess} |         |         |
|         |         | "Sign   |         |         |         |         |
|         |         | in"     |         |         |         |         |
|         |         | button  |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| Main-3  | Sign in | Enter   | Show an | [PASS]  |         |         |
|         |         | invalid | error   | {.statu |         |         |
|         |         | p       | message | s-macro |         |         |
|         |         | assword | "       | .aui-   |         |         |
|         |         |         | Invalid | lozenge |         |         |
|         |         |         | Pa      | .aui-lo |         |         |
|         |         |         | ssword" | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| Main-4  | Create  | Click   | Go to   | [PASS]  |         |         |
|         | New     | on      | screen  | {.statu |         |         |
|         | Account | "Create | "Create | s-macro |         |         |
|         | Wallet  | Account | Wallet" | .aui-   |         |         |
|         |         | Wallet" | with 3  | lozenge |         |         |
|         |         | button  | se      | .aui-lo |         |         |
|         |         |         | lection | zenge-s |         |         |
|         |         |         | types   | uccess} |         |         |
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
| .1.7-1- |         |         |         |         |         |         |
| SignIn} |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| S       | P       | Leave   | Show    | [PASS]  |         |         |
| IGNIN-1 | assword | the     | r       | {.statu |         |         |
|         |         | field   | equired | s-macro |         |         |
|         |         | empty   | field   | .aui-   |         |         |
|         |         |         | message | lozenge |         |         |
|         |         |         | "P      | .aui-lo |         |         |
|         |         |         | assword | zenge-s |         |         |
|         |         |         | is      | uccess} |         |         |
|         |         |         | re      |         |         |         |
|         |         |         | quired" |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| S       |         | Place   | Show    | [FAIL]  | It      |         |
| IGNIN-2 |         | less    | message | {.statu | shows   |         |
|         |         | than    | of      | s-macro | "p      |         |
|         |         | r       | minimum | .aui-   | assword |         |
|         |         | equired | number  | lozenge | is      |         |
|         |         | values  | of      | .aui-   | re      |         |
|         |         |         | cha     | lozenge | quired" |         |
|         |         |         | racters | -error} | instead |         |
|         |         |         | to      |         |         |         |
|         |         |         | enter   |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| S       |         | Enter   | Show an | [PASS]  |         |         |
| IGNIN-3 |         | invalid | error   | {.statu |         |         |
|         |         | p       | message | s-macro |         |         |
|         |         | assword | "       | .aui-   |         |         |
|         |         |         | Invalid | lozenge |         |         |
|         |         |         | Pa      | .aui-lo |         |         |
|         |         |         | ssword" | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| S       | After   | Click   | Enter   | [PASS]  |         |         |
| IGNIN-4 | se      | o       | the     | {.statu |         |         |
|         | lecting | n "Sign | appl    | s-macro |         |         |
|         | wallet  | in"     | ication | .aui-   |         |         |
|         | and     | button  | (main   | lozenge |         |         |
|         | e       |         | home    | .aui-lo |         |         |
|         | ntering |         | page of | zenge-s |         |         |
|         | p       |         | Sirius  | uccess} |         |         |
|         | assword |         | Wallet) |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| S       | Sign    | Click   | Go back | [PASS]  |         |         |
| IGNIN-5 | Out     | on      | to Sign | {.statu |         |         |
|         |         | "Sign   | In page | s-macro |         |         |
|         |         | Out"    |         | .aui-   |         |         |
|         |         | button  |         | lozenge |         |         |
|         |         |         |         | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ###     |         |         |         |         |         |         |
|  Create |         |         |         |         |         |         |
|  New Wa |         |         |         |         |         |         |
| llet {# |         |         |         |         |         |         |
| TestRep |         |         |         |         |         |         |
| ort-1.1 |         |         |         |         |         |         |
| .7-1-Cr |         |         |         |         |         |         |
| eateNew |         |         |         |         |         |         |
| Wallet} |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| N       | Create\ | Click   | Go to   | [PASS]  |         |         |
| EWWLT-1 | (New    | on      | screen  | {.statu |         |         |
|         | Wallet) | Create  | "Create | s-macro |         |         |
|         |         | "New    | Wallet  | .aui-   |         |         |
|         |         | Wallet" | "       | lozenge |         |         |
|         |         | button  |         | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| N       | Wallet  | Leave   | Show a  | [PASS]  |         |         |
| EWWLT-2 | name    | the     | message | {.statu |         |         |
|         |         | field   | "Enter  | s-macro |         |         |
|         |         | empty   | Wallet  | .aui-   |         |         |
|         |         |         | Name"   | lozenge |         |         |
|         |         |         |         | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| N       |         | Set     | N/A     | [PASS]  |         |         |
| EWWLT-3 |         | special |         | {.statu |         |         |
|         |         | cha     |         | s-macro |         |         |
|         |         | racters |         | .aui-   |         |         |
|         |         |         |         | lozenge |         |         |
|         |         |         |         | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| N       | Pa      | Leave   | Show an | [PASS]  |         |         |
| EWWLT-4 | ssword  | the     | error   | {.statu |         |         |
|         |         | field   | message | s-macro |         |         |
|         |         | empty   |         | .aui-   |         |         |
|         |         |         |         | lozenge |         |         |
|         |         |         |         | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| N       |         | Set an  | Show a  | [PASS]  |         |         |
| EWWLT-5 |         | invalid | message | {.statu |         |         |
|         |         | p       | "min    | s-macro |         |         |
|         |         | assword | length  | .aui-   |         |         |
|         |         |         | 8"      | lozenge |         |         |
|         |         |         |         | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| N       |         | Set     | special | [PASS]  |         |         |
| EWWLT-6 |         | special | cha     | {.statu |         |         |
|         |         | cha     | racters | s-macro |         |         |
|         |         | racters | can be  | .aui-   |         |         |
|         |         |         | used    | lozenge |         |         |
|         |         |         | for     | .aui-lo |         |         |
|         |         |         | p       | zenge-s |         |         |
|         |         |         | assword | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| N       |         | Place   | Show    | [PASS]  |         |         |
| EWWLT-7 |         | less    | message | {.statu |         |         |
|         |         | than    | of      | s-macro |         |         |
|         |         | r       | minimum | .aui-   |         |         |
|         |         | equired | number  | lozenge |         |         |
|         |         | values  | of      | .aui-lo |         |         |
|         |         |         | cha     | zenge-s |         |         |
|         |         |         | racters | uccess} |         |         |
|         |         |         | to      |         |         |         |
|         |         |         | enter\  |         |         |         |
|         |         |         | "min    |         |         |         |
|         |         |         | length  |         |         |         |
|         |         |         | 8"      |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| N       | Confirm | Leave   | Show a  | [PASS]  |         |         |
| EWWLT-8 | p       | the     | m       | {.statu |         |         |
|         | assword | field   | essage\ | s-macro |         |         |
|         |         | empty   | "P      | .aui-   |         |         |
|         |         |         | assword | lozenge |         |         |
|         |         |         | doesn't | .aui-lo |         |         |
|         |         |         | match"  | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| N       |         | Enter a | Show a  | [PASS]  |         |         |
| EWWLT-9 |         | di      | m       | {.statu |         |         |
|         |         | fferent | essage\ | s-macro |         |         |
|         |         | p       | "P      | .aui-   |         |         |
|         |         | assword | assword | lozenge |         |         |
|         |         |         | doesn't | .aui-lo |         |         |
|         |         |         | match"  | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Set     | special | [PASS]  |         |         |
| WWLT-10 |         | special | cha     | {.statu |         |         |
|         |         | cha     | racters | s-macro |         |         |
|         |         | racters | can be  | .aui-   |         |         |
|         |         |         | used    | lozenge |         |         |
|         |         |         | for     | .aui-lo |         |         |
|         |         |         | p       | zenge-s |         |         |
|         |         |         | assword | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Place   | Show a  | [PASS]  |         |         |
| WWLT-11 |         | less or | m       | {.statu |         |         |
|         |         | more    | essage\ | s-macro |         |         |
|         |         | than    | "P      | .aui-   |         |         |
|         |         | r       | assword | lozenge |         |         |
|         |         | equired | doesn't | .aui-lo |         |         |
|         |         | values  | match"  | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      | Eye     | Click   | Show /  | [PASS]  |         |         |
| WWLT-12 | Icons   | on      | hide    | {.statu |         |         |
|         |         | "Pa     | the     | s-macro |         |         |
|         |         | ssword" | p       | .aui-   |         |         |
|         |         | eye     | assword | lozenge |         |         |
|         |         | icon    |         | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Click   | Show /  | [PASS]  |         |         |
| WWLT-13 |         | on      | hide    | {.statu |         |         |
|         |         | "       | the     | s-macro |         |         |
|         |         | Confirm | p       | .aui-   |         |         |
|         |         | pa      | assword | lozenge |         |         |
|         |         | ssword" |         | .aui-lo |         |         |
|         |         | eye     |         | zenge-s |         |         |
|         |         | icon    |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      | Create  | Click   | Send a  | [PASS]  |         |         |
| WWLT-14 |         | on      | confi   | {.statu |         |         |
|         |         | "Create | rmation | s-macro |         |         |
|         |         | Wallet" | message | .aui-   |         |         |
|         |         | button  | and     | lozenge |         |         |
|         |         |         | create  | .aui-lo |         |         |
|         |         |         | the     | zenge-s |         |         |
|         |         |         | wallet  | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ### Cr  |         |         |         |         |         |         |
| eate Ne |         |         |         |         |         |         |
| w Walle |         |         |         |         |         |         |
| t From  |         |         |         |         |         |         |
| Private |         |         |         |         |         |         |
|  Key {# |         |         |         |         |         |         |
| TestRep |         |         |         |         |         |         |
| ort-1.1 |         |         |         |         |         |         |
| .7-1-Cr |         |         |         |         |         |         |
| eateNew |         |         |         |         |         |         |
| WalletF |         |         |         |         |         |         |
| romPriv |         |         |         |         |         |         |
| ateKey} |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      | Create  | Click   | Go to   | [PASS]  |         |         |
| WWLT-15 | Wallet\ | on      | screen  | {.statu |         |         |
|         | (From a | Create  | "Create | s-macro |         |         |
|         | Private | Wallet  | Wallet  | .aui-   |         |         |
|         | Key)    | "From a | from a  | lozenge |         |         |
|         |         | Private | Private | .aui-lo |         |         |
|         |         | Key"    | Key"    | zenge-s |         |         |
|         |         | button  |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      | Private | Leave   | Show an | [PASS]  |         |         |
| WWLT-16 | key     | the     | error   | {.statu |         |         |
|         |         | field   | message | s-macro |         |         |
|         |         | empty   | "       | .aui-   |         |         |
|         |         |         | Invalid | lozenge |         |         |
|         |         |         | private | .aui-lo |         |         |
|         |         |         | key"    | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Set an  | Show an | [PASS]  |         |         |
| WWLT-17 |         | invalid | error   | {.statu |         |         |
|         |         | value   | message | s-macro |         |         |
|         |         |         | "       | .aui-   |         |         |
|         |         |         | Invalid | lozenge |         |         |
|         |         |         | private | .aui-lo |         |         |
|         |         |         | key"    | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      | Wallet  | Leave   | Show a  | [PASS]  |         |         |
| WWLT-18 | name    | the     | message | {.statu |         |         |
|         |         | field   | "Enter  | s-macro |         |         |
|         |         | empty   | Wallet  | .aui-   |         |         |
|         |         |         | Name"   | lozenge |         |         |
|         |         |         |         | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Set     | N/A     | [PASS]  |         |         |
| WWLT-19 |         | special |         | {.statu |         |         |
|         |         | cha     |         | s-macro |         |         |
|         |         | racters |         | .aui-   |         |         |
|         |         |         |         | lozenge |         |         |
|         |         |         |         | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      | Pa      | Leave   | Show a  | [PASS]  |         |         |
| WWLT-20 | ssword  | the     | message | {.statu |         |         |
|         |         | field   | "min    | s-macro |         |         |
|         |         | empty   | length  | .aui-   |         |         |
|         |         |         | 8"      | lozenge |         |         |
|         |         |         |         | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Set an  | Show a  | [PASS]  |         |         |
| WWLT-21 |         | invalid | message | {.statu |         |         |
|         |         | p       | "min    | s-macro |         |         |
|         |         | assword | length  | .aui-   |         |         |
|         |         |         | 8"      | lozenge |         |         |
|         |         |         |         | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Set     | N/A     | [PASS]  |         |         |
| WWLT-22 |         | special |         | {.statu |         |         |
|         |         | cha     |         | s-macro |         |         |
|         |         | racters |         | .aui-   |         |         |
|         |         |         |         | lozenge |         |         |
|         |         |         |         | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Place   | Show    | [PASS]  |         |         |
| WWLT-23 |         | less    | message | {.statu |         |         |
|         |         | than    | of      | s-macro |         |         |
|         |         | r       | minimum | .aui-   |         |         |
|         |         | equired | number  | lozenge |         |         |
|         |         | values  | of      | .aui-lo |         |         |
|         |         |         | cha     | zenge-s |         |         |
|         |         |         | racters | uccess} |         |         |
|         |         |         | to      |         |         |         |
|         |         |         | enter\  |         |         |         |
|         |         |         | "min    |         |         |         |
|         |         |         | length  |         |         |         |
|         |         |         | 8"      |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      | Confirm | Leave   | Show a  | [PASS]  |         |         |
| WWLT-24 | p       | the     | message | {.statu |         |         |
|         | assword | field   | "P      | s-macro |         |         |
|         |         | empty   | assword | .aui-   |         |         |
|         |         |         | doesn't | lozenge |         |         |
|         |         |         | match"  | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Enter a | Show a  | [PASS]  |         |         |
| WWLT-25 |         | di      | message | {.statu |         |         |
|         |         | fferent | "P      | s-macro |         |         |
|         |         | p       | assword | .aui-   |         |         |
|         |         | assword | doesn't | lozenge |         |         |
|         |         |         | match"  | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Set     | N/A     | [PASS]  |         | \-      |
| WWLT-26 |         | special |         | {.statu |         |         |
|         |         | cha     |         | s-macro |         |         |
|         |         | racters |         | .aui-   |         |         |
|         |         |         |         | lozenge |         |         |
|         |         |         |         | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Place   | Show a  | [PASS]  |         |         |
| WWLT-27 |         | less or | message | {.statu |         |         |
|         |         | more    | "P      | s-macro |         |         |
|         |         | than    | assword | .aui-   |         |         |
|         |         | r       | doesn't | lozenge |         |         |
|         |         | equired | match"\ | .aui-lo |         |         |
|         |         | values  |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      | Eye     | Click   | Show /  | [PASS]  |         |         |
| WWLT-28 | icons   | on      | hide    | {.statu |         |         |
|         |         | "       | the     | s-macro |         |         |
|         |         | Private | private | .aui-   |         |         |
|         |         | key"    | key     | lozenge |         |         |
|         |         | eye     |         | .aui-lo |         |         |
|         |         | icon    |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Click   | Show /  | [PASS]  |         |         |
| WWLT-29 |         | on      | hide    | {.statu |         |         |
|         |         | "Pa     | the     | s-macro |         |         |
|         |         | ssword" | p       | .aui-   |         |         |
|         |         | eye     | assword | lozenge |         |         |
|         |         | icon    |         | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Click   | Show /  | [PASS]  |         |         |
| WWLT-30 |         | on      | hide    | {.statu |         |         |
|         |         | "       | the     | s-macro |         |         |
|         |         | Confirm | p       | .aui-   |         |         |
|         |         | pa      | assword | lozenge |         |         |
|         |         | ssword" |         | .aui-lo |         |         |
|         |         | eye     |         | zenge-s |         |         |
|         |         | icon    |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      | N/A     | Click   | Send a  | [PASS]  |         |         |
| WWLT-31 |         | on      | confi   | {.statu |         |         |
|         |         | "       | rmation | s-macro |         |         |
|         |         | Create" | message | .aui-   |         |         |
|         |         | button  | and     | lozenge |         |         |
|         |         |         | create  | .aui-lo |         |         |
|         |         |         | the     | zenge-s |         |         |
|         |         |         | wallet  | uccess} |         |         |
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
| .1.7-1- |         |         |         |         |         |         |
| Importw |         |         |         |         |         |         |
| alletfr |         |         |         |         |         |         |
| om.wltf |         |         |         |         |         |         |
| ile(Cre |         |         |         |         |         |         |
| ateWall |         |         |         |         |         |         |
| etfroma |         |         |         |         |         |         |
| WalletB |         |         |         |         |         |         |
| ackup)} |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      | Import\ | Click   | Go to   | [PASS]  |         |         |
| WWLT-32 | (From a | on      | screen  | {.statu |         |         |
|         | Wallet  | "From a | "Create | s-macro |         |         |
|         | Backup) | wallet  | Wallet  | .aui-   |         |         |
|         |         | backup" | from a  | lozenge |         |         |
|         |         | button  | Wallet  | .aui-lo |         |         |
|         |         |         | Backup" | zenge-s |         |         |
|         |         |         | and     | uccess} |         |         |
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
| NE      |         | Already | Go back | [PASS]  |         |         |
| WWLT-33 |         | have a  | to Sign | {.statu |         |         |
|         |         | Sirius  | In page | s-macro |         |         |
|         |         | Wallet  |         | .aui-   |         |         |
|         |         | a       |         | lozenge |         |         |
|         |         | ccount, |         | .aui-lo |         |         |
|         |         | click   |         | zenge-s |         |         |
|         |         | on      |         | uccess} |         |         |
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
| 7-1-Das |         |         |         |         |         |         |
| hboard} |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| **Test  | **Test  | **Test  | **E     | **S     | **R     | **Auto  |
| Case    | Scen    | steps** | xpected | tatus** | emark** | mated** |
| ID**    | arios** |         | r       |         |         |         |
|         |         |         | esult** |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-1  | Home    | Click   | Back to | [PASS]  |         |         |
|         |         | "Home"  | da      | {.statu |         |         |
|         |         | icon    | shboard | s-macro |         |         |
|         |         |         | home    | .aui-   |         |         |
|         |         |         | page    | lozenge |         |         |
|         |         |         |         | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-2  | +New    | Click   | Users   | [PASS]  |         |         |
|         |         | "+New"  | can     | {.statu |         |         |
|         |         | button  | select  | s-macro |         |         |
|         |         |         | to      | .aui-   |         |         |
|         |         |         | t       | lozenge |         |         |
|         |         |         | ransfer | .aui-lo |         |         |
|         |         |         | xpx,    | zenge-s |         |         |
|         |         |         | create  | uccess} |         |         |
|         |         |         | digital |         |         |         |
|         |         |         | asset,  |         |         |         |
|         |         |         | na      |         |         |         |
|         |         |         | mespace |         |         |         |
|         |         |         | and     |         |         |         |
|         |         |         | account |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-3  |         | After   | User    | [PASS]  |         |         |
|         |         | c       | d       | {.statu |         |         |
|         |         | licking | irected | s-macro |         |         |
|         |         | new     | to      | .aui-   |         |         |
|         |         | button, | create  | lozenge |         |         |
|         |         | click   | asset   | .aui-lo |         |         |
|         |         | digital | page    | zenge-s |         |         |
|         |         | asset   |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-4  |         | After   | User    | [PASS]  |         |         |
|         |         | c       | d       | {.statu |         |         |
|         |         | licking | irected | s-macro |         |         |
|         |         | new     | to      | .aui-   |         |         |
|         |         | button, | create  | lozenge |         |         |
|         |         | click   | na      | .aui-lo |         |         |
|         |         | na      | mespace | zenge-s |         |         |
|         |         | mespace | page    | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-5  |         | After   | User    | [PASS]  |         |         |
|         |         | c       | d       | {.statu |         |         |
|         |         | licking | irected | s-macro |         |         |
|         |         | new     | to      | .aui-   |         |         |
|         |         | button, | create  | lozenge |         |         |
|         |         | click   | account | .aui-lo |         |         |
|         |         | account | page    | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
|         |         | After   | User    | [PASS]  |         |         |
|         |         | c       | d       | {.statu |         |         |
|         |         | licking | irected | s-macro |         |         |
|         |         | new     | to      | .aui-   |         |         |
|         |         | button, | t       | lozenge |         |         |
|         |         | click   | ransfer | .aui-lo |         |         |
|         |         | t       | xpx     | zenge-s |         |         |
|         |         | ransfer | page    | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-6  | Beg     | Click   | A list  | [PASS]  |         |         |
|         | inner's | on      | of      | {.statu |         |         |
|         | guide   | q       | b       | s-macro |         |         |
|         |         | uestion | eginner | .aui-   |         |         |
|         |         | mark    | guides  | lozenge |         |         |
|         |         | button  | av      | .aui-lo |         |         |
|         |         |         | ailable | zenge-s |         |         |
|         |         |         | for     | uccess} |         |         |
|         |         |         | user    |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-7  | Notif   | Click   | User    | [PASS]  |         |         |
|         | ication | on      | d       | {.statu |         |         |
|         |         | notif   | irected | s-macro |         |         |
|         |         | ication | to      | .aui-   |         |         |
|         |         | button  | notif   | lozenge |         |         |
|         |         |         | ication | .aui-lo |         |         |
|         |         |         | page    | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-8  | S       | Click   | User    | [PASS]  |         |         |
|         | ettings | on      | d       | {.statu |         |         |
|         |         | s       | irected | s-macro |         |         |
|         |         | ettings | to      | .aui-   |         |         |
|         |         | button  | s       | lozenge |         |         |
|         |         |         | ettings | .aui-lo |         |         |
|         |         |         | page    | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
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
|         |         |         |         |         | 9911705 |         |
|         |         |         |         |         | 7_5b142 |         |
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
|         |         |         |         |         | 9911705 |         |
|         |         |         |         |         | 7_5b142 |         |
|         |         |         |         |         | d79091e |         |
|         |         |         |         |         | 9f17116 |         |
|         |         |         |         |         | 363a5"} |         |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-10 | Assets  | Click   | D       | [PASS]  |         |         |
|         |         | on      | isplays | {.statu |         |         |
|         |         | "       | a list  | s-macro |         |         |
|         |         | Assets" | of      | .aui-   |         |         |
|         |         | tab     | user's  | lozenge |         |         |
|         |         |         | assets  | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-11 | Nam     | Click   | D       | [PASS]  |         |         |
|         | espaces | on      | isplays | {.statu |         |         |
|         |         | "Name   | a list  | s-macro |         |         |
|         |         | spaces" | of      | .aui-   |         |         |
|         |         | tab     | user's  | lozenge |         |         |
|         |         |         | nam     | .aui-lo |         |         |
|         |         |         | espaces | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-12 | All     | Click   | D       | [PASS]  |         |         |
|         | Trans   | on "All | isplays | {.statu |         |         |
|         | actions | transa  | a list  | s-macro |         |         |
|         |         | ctions" | of      | .aui-   |         |         |
|         |         | tab     | user's  | lozenge |         |         |
|         |         |         | trans   | .aui-lo |         |         |
|         |         |         | actions | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-13 | Header  | Click   | Wallet  | [PASS]  |         |         |
|         | com     | on copy | address | {.statu |         |         |
|         | ponents | wallet  | is      | s-macro |         |         |
|         |         | address | copied  | .aui-   |         |         |
|         |         | button  | and a   | lozenge |         |         |
|         |         |         | notif   | .aui-lo |         |         |
|         |         |         | ication | zenge-s |         |         |
|         |         |         | is      | uccess} |         |         |
|         |         |         | shown   |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-14 |         | Click   | User    | [PASS]  |         |         |
|         |         | on      | d       | {.statu |         |         |
|         |         | "Swap"  | irected | s-macro |         |         |
|         |         | button  | to swap | .aui-   |         |         |
|         |         |         | page    | lozenge |         |         |
|         |         |         |         | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-15 |         | Click   | Display | [PASS]  |         |         |
|         |         | on      | QR Code | {.statu |         |         |
|         |         | "Scan   | of      | s-macro |         |         |
|         |         | QR      | wallet  | .aui-   |         |         |
|         |         | Code"   | address | lozenge |         |         |
|         |         | button  |         | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-16 |         | Click   | User    | [PASS]  |         |         |
|         |         | on      | d       | {.statu |         |         |
|         |         | "       | irected | s-macro |         |         |
|         |         | Convert | to      | .aui-   |         |         |
|         |         | to      | m       | lozenge |         |         |
|         |         | Mu      | ultisig | .aui-lo |         |         |
|         |         | ltisig" | page    | zenge-s |         |         |
|         |         | button  |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-17 |         | Click   | User is | [PASS]  |         |         |
|         |         | on      | d       | {.statu |         |         |
|         |         | "T      | irected | s-macro |         |         |
|         |         | ransfer | to      | .aui-   |         |         |
|         |         | XPX"    | t       | lozenge |         |         |
|         |         | button  | ransfer | .aui-lo |         |         |
|         |         |         | xpx     | zenge-s |         |         |
|         |         |         | page    | uccess} |         |         |
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
| 1.7-1-S |         |         |         |         |         |         |
| ideMenu |         |         |         |         |         |         |
| Bar(Hom |         |         |         |         |         |         |
| ePage)} |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| **Test  | **Test  | **Test  | **E     | **S     | **R     | **Auto  |
| Case    | Scen    | steps** | xpected | tatus** | emark** | mated** |
| ID**    | arios** |         | r       |         |         |         |
|         |         |         | esult** |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-1  | Account | Click   | User is | [PASS]  |         |         |
|         |         | on any  | d       | {.statu |         |         |
|         |         | account | irected | s-macro |         |         |
|         |         | under   | to the  | .aui-   |         |         |
|         |         | "Ac     | res     | lozenge |         |         |
|         |         | counts" | pective | .aui-lo |         |         |
|         |         |         | account | zenge-s |         |         |
|         |         |         | details | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-2  | Create  | Click   | User is | [PASS]  |         |         |
|         | New     | on      | d       | {.statu |         |         |
|         | Account | "       | irected | s-macro |         |         |
|         |         | +Create | to      | .aui-   |         |         |
|         |         | New     | "Create | lozenge |         |         |
|         |         | A       | New     | .aui-lo |         |         |
|         |         | ccount" | A       | zenge-s |         |         |
|         |         | under   | ccount" | uccess} |         |         |
|         |         | "       | Page    |         |         |         |
|         |         | Default |         |         |         |         |
|         |         | A       |         |         |         |         |
|         |         | ccount" |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-3  | Na      | Click   | User is | [PASS]  |         |         |
|         | mespace | on      | d       | {.statu |         |         |
|         |         | "Nam    | irected | s-macro |         |         |
|         |         | espace" | to a    | .aui-   |         |         |
|         |         | under   | page to | lozenge |         |         |
|         |         | "Quick  | create  | .aui-lo |         |         |
|         |         | Action" | na      | zenge-s |         |         |
|         |         |         | mespace | uccess} |         |         |
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
|         |         |         |         |         | 9911705 |         |
|         |         |         |         |         | 7_5b142 |         |
|         |         |         |         |         | d79091e |         |
|         |         |         |         |         | 9f17116 |         |
|         |         |         |         |         | 363a5"} |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-6  |         | Enter   | Shows   | [PASS]  |         |         |
|         |         | invalid | an      | {.statu |         |         |
|         |         | name    | error   | s-macro |         |         |
|         |         | (one    | message | .aui-   |         |         |
|         |         | char)   | to      | lozenge |         |         |
|         |         |         | enter   | .aui-lo |         |         |
|         |         |         | valid   | zenge-s |         |         |
|         |         |         | name    | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-7  |         | Enter   | Na      | [PASS]  |         |         |
|         |         | valid   | mespace | {.statu |         |         |
|         |         | name,\  | created | s-macro |         |         |
|         |         | Enter   | with id | .aui-   |         |         |
|         |         | d       | and     | lozenge |         |         |
|         |         | uration | exp     | .aui-lo |         |         |
|         |         | of      | iration | zenge-s |         |         |
|         |         | days,\  | ti      | uccess} |         |         |
|         |         | Enter   | mestamp |         |         |         |
|         |         | correct |         |         |         |         |
|         |         | p       |         |         |         |         |
|         |         | assword |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-8  |         | Enter   | User is | [PASS]  |         |         |
|         |         | valid   | d       | {.statu |         |         |
|         |         | name,\  | irected | s-macro |         |         |
|         |         | Enter   | back to | .aui-   |         |         |
|         |         | d       | na      | lozenge |         |         |
|         |         | uration | mespace | .aui-lo |         |         |
|         |         | of      | page    | zenge-s |         |         |
|         |         | days,\  |         | uccess} |         |         |
|         |         | Enter   |         |         |         |         |
|         |         | correct |         |         |         |         |
|         |         | pas     |         |         |         |         |
|         |         | sword,\ |         |         |         |         |
|         |         | Click   |         |         |         |         |
|         |         | "       |         |         |         |         |
|         |         | Cancel" |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-9  |         | Enter   | Shows   | [PASS]  |         |         |
|         |         | valid   | an      | {.statu |         |         |
|         |         | name,\  | error   | s-macro |         |         |
|         |         | Enter   | saying  | .aui-   |         |         |
|         |         | d       | p       | lozenge |         |         |
|         |         | uration | assword | .aui-lo |         |         |
|         |         | of      | is      | zenge-s |         |         |
|         |         | days,\  | r       | uccess} |         |         |
|         |         | Leave   | equired |         |         |         |
|         |         | p       | and     |         |         |         |
|         |         | assword | r       |         |         |         |
|         |         | empty   | egister |         |         |         |
|         |         |         | button  |         |         |         |
|         |         |         | is      |         |         |         |
|         |         |         | d       |         |         |         |
|         |         |         | isabled |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-10 |         | Enter   | Shows   | [PASS]  |         |         |
|         |         | wrong   | an      | {.statu |         |         |
|         |         | wallet  | error   | s-macro |         |         |
|         |         | p       | saying  | .aui-   |         |         |
|         |         | assword | wallet  | lozenge |         |         |
|         |         |         | p       | .aui-lo |         |         |
|         |         |         | assword | zenge-s |         |         |
|         |         |         | is      | uccess} |         |         |
|         |         |         | in      |         |         |         |
|         |         |         | correct |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-11 | Asset   | Click   | User is | [PASS]  |         |         |
|         |         | on      | d       | {.statu |         |         |
|         |         | "Asset" | irected | s-macro |         |         |
|         |         | under   | to      | .aui-   |         |         |
|         |         | "Quick  | "       | lozenge |         |         |
|         |         | Action" | Assets" | .aui-lo |         |         |
|         |         |         | page    | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-12 |         | Click   | User is | [PASS]  |         |         |
|         |         | on      | d       | {.statu |         |         |
|         |         | "       | irected | s-macro |         |         |
|         |         | +Create | to      | .aui-   |         |         |
|         |         | New     | "Create | lozenge |         |         |
|         |         | Asset"  | Asset"  | .aui-lo |         |         |
|         |         |         | page    | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-13 |         | Leave   | Show an | [PASS]  |         |         |
|         |         | supply, | error   | {.statu |         |         |
|         |         | divis   | to      | s-macro |         |         |
|         |         | ibility | enter   | .aui-   |         |         |
|         |         | and     | wallet  | lozenge |         |         |
|         |         | wallet  | p       | .aui-lo |         |         |
|         |         | p       | assword | zenge-s |         |         |
|         |         | assword |         | uccess} |         |         |
|         |         | empty   |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-14 |         | Enter   | Asset   | [PASS]  |         |         |
|         |         | amount  | is      | {.statu |         |         |
|         |         | of      | created | s-macro |         |         |
|         |         | s       | with    | .aui-   |         |         |
|         |         | upply,\ | its     | lozenge |         |         |
|         |         | Enter   | res     | .aui-lo |         |         |
|         |         | divisib | pective | zenge-s |         |         |
|         |         | ility,\ | id and  | uccess} |         |         |
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
|         |         |         |         |         | 9911705 |         |
|         |         |         |         |         | 7_5b142 |         |
|         |         |         |         |         | d79091e |         |
|         |         |         |         |         | 9f17116 |         |
|         |         |         |         |         | 363a5"} |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-16 | Wallets | Click   | D       | [PASS]  |         |         |
|         |         | on      | isplays | {.statu |         |         |
|         |         | "W      | a list  | s-macro |         |         |
|         |         | allets" | of      | .aui-   |         |         |
|         |         | under   | wallets | lozenge |         |         |
|         |         | "Na     | av      | .aui-lo |         |         |
|         |         | vigate" | ailable | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-17 |         | Click   | D       | [PASS]  |         |         |
|         |         | on the  | isplays | {.statu |         |         |
|         |         | trash   | the     | s-macro |         |         |
|         |         | icon of | delete  | .aui-   |         |         |
|         |         | the     | confi   | lozenge |         |         |
|         |         | wallet  | rmation | .aui-lo |         |         |
|         |         | to      | pop-up  | zenge-s |         |         |
|         |         | delete  |         | uccess} |         |         |
|         |         | it      |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-18 |         | Click   | Wallet  | [PASS]  |         |         |
|         |         | on      | succe   | {.statu |         |         |
|         |         | delete  | ssfully | s-macro |         |         |
|         |         | now     | removed | .aui-   |         |         |
|         |         | button  | and a   | lozenge |         |         |
|         |         |         | notif   | .aui-lo |         |         |
|         |         |         | ication | zenge-s |         |         |
|         |         |         | is      | uccess} |         |         |
|         |         |         | shown   |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-19 | A       | Click   | D       | [PASS]  |         |         |
|         | ccounts | on      | isplays | {.statu |         |         |
|         |         | "Ac     | an      | s-macro |         |         |
|         |         | counts" | o       | .aui-   |         |         |
|         |         | under   | verview | lozenge |         |         |
|         |         | "Na     | of the  | .aui-lo |         |         |
|         |         | vigate" | user's  | zenge-s |         |         |
|         |         |         | a       | uccess} |         |         |
|         |         |         | ccounts |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-20 |         | Click   | D       | [PASS]  |         |         |
|         |         | on "My  | isplays | {.statu |         |         |
|         |         | Ac      | user's  | s-macro |         |         |
|         |         | counts" | a       | .aui-   |         |         |
|         |         | tab     | ccounts | lozenge |         |         |
|         |         |         |         | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-21 |         | Click   | D       | [PASS]  |         |         |
|         |         | on      | isplays | {.statu |         |         |
|         |         | "M      | user's  | s-macro |         |         |
|         |         | ultisig | m       | .aui-   |         |         |
|         |         | Ac      | ultisig | lozenge |         |         |
|         |         | counts" | a       | .aui-lo |         |         |
|         |         | tab     | ccounts | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-22 |         | Click   | D       | [PASS]  |         |         |
|         |         | on      | isplays | {.statu |         |         |
|         |         | "Other  | user's  | s-macro |         |         |
|         |         | Ac      | other   | .aui-   |         |         |
|         |         | counts" | a       | lozenge |         |         |
|         |         | tab     | ccounts | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-23 | Address | Click   | D       | [PASS]  |         |         |
|         | Book    | on      | isplays | {.statu |         |         |
|         |         | "       | user's  | s-macro |         |         |
|         |         | Address | address | .aui-   |         |         |
|         |         | Book"   | book    | lozenge |         |         |
|         |         | under   | list    | .aui-lo |         |         |
|         |         | "Na     |         | zenge-s |         |         |
|         |         | vigate" |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-24 |         | Click   | User    | [PASS]  |         |         |
|         |         | on      | d       | {.statu |         |         |
|         |         | "+Add   | irected | s-macro |         |         |
|         |         | New     | to "Add | .aui-   |         |         |
|         |         | A       | New     | lozenge |         |         |
|         |         | ddress" | C       | .aui-lo |         |         |
|         |         |         | ontact" | zenge-s |         |         |
|         |         |         | page    | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-25 |         | Enter   | Shows a | [PASS]  |         |         |
|         |         | valid   | message | {.statu |         |         |
|         |         | ad      | saying  | s-macro |         |         |
|         |         | dress,\ | name is | .aui-   |         |         |
|         |         | Leave   | r       | lozenge |         |         |
|         |         | name    | equired | .aui-lo |         |         |
|         |         | empty   |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-26 |         | Enter   | Show an | [PASS]  |         |         |
|         |         | name,\  | error   | {.statu |         |         |
|         |         | Enter   | (       | s-macro |         |         |
|         |         | invalid | address | .aui-   |         |         |
|         |         | address | is      | lozenge |         |         |
|         |         |         | re      | .aui-lo |         |         |
|         |         |         | quired) | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-27 |         | Enter   | Shows a | [PASS]  |         |         |
|         |         | name,   | message | {.statu |         |         |
|         |         | place   | saying  | s-macro |         |         |
|         |         | less or | address | .aui-   |         |         |
|         |         | more    | is      | lozenge |         |         |
|         |         | than    | r       | .aui-lo |         |         |
|         |         | r       | equired | zenge-s |         |         |
|         |         | equired |         | uccess} |         |         |
|         |         | value   |         |         |         |         |
|         |         | for     |         |         |         |         |
|         |         | address |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-28 |         | Enter   | Shows a | [PASS]  |         |         |
|         |         | an      | message | {.statu |         |         |
|         |         | address | saying  | s-macro |         |         |
|         |         | that    | the     | .aui-   |         |         |
|         |         | already | address | lozenge |         |         |
|         |         | exists  | exists  | .aui-lo |         |         |
|         |         | in the  | in the  | zenge-s |         |         |
|         |         | wallet  | wallet  | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-29 |         | Enter   | New     | [PASS]  |         |         |
|         |         | name,\  | address | {.statu |         |         |
|         |         | Enter   | added   | s-macro |         |         |
|         |         | valid   | and     | .aui-   |         |         |
|         |         | ad      | di      | lozenge |         |         |
|         |         | dress,\ | splayed | .aui-lo |         |         |
|         |         | Click   | under   | zenge-s |         |         |
|         |         | save    | address | uccess} |         |         |
|         |         | address | book    |         |         |         |
|         |         |         | list    |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-30 | Custom  | Enter   | Enter   | [PASS]  |         |         |
|         |         | name,\  | custom  | {.statu |         |         |
|         |         | Enter   | group   | s-macro |         |         |
|         |         | valid   | name    | .aui-   |         |         |
|         |         | ad      | pop up  | lozenge |         |         |
|         |         | dress,\ | is      | .aui-lo |         |         |
|         |         | Choose  | shown   | zenge-s |         |         |
|         |         | custom  |         | uccess} |         |         |
|         |         | group   |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-31 |         | Enter   | New     | [PASS]  |         |         |
|         |         | valid   | address | {.statu |         |         |
|         |         | custom  | added   | s-macro |         |         |
|         |         | group   | and     | .aui-   |         |         |
|         |         | name,   | di      | lozenge |         |         |
|         |         | save    | splayed | .aui-lo |         |         |
|         |         | address | under   | zenge-s |         |         |
|         |         |         | address | uccess} |         |         |
|         |         |         | book    |         |         |         |
|         |         |         | list    |         |         |         |
|         |         |         | with    |         |         |         |
|         |         |         | the     |         |         |         |
|         |         |         | custom  |         |         |         |
|         |         |         | group   |         |         |         |
|         |         |         | name    |         |         |         |
|         |         |         | created |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-32 | Edit    | Click   | User    | [PASS]  |         |         |
|         | address | on edit | d       | {.statu |         |         |
|         |         | address | irected | s-macro |         |         |
|         |         |         | to edit | .aui-   |         |         |
|         |         |         | contact | lozenge |         |         |
|         |         |         | page    | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-33 |         | Edit    | Show an | [PASS]  |         |         |
|         |         | name    | error   | {.statu |         |         |
|         |         | field   |         | s-macro |         |         |
|         |         | to be   |         | .aui-   |         |         |
|         |         | empty   |         | lozenge |         |         |
|         |         |         |         | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-34 |         | Edit    | Show an | [PASS]  |         |         |
|         |         | address | error   | {.statu |         |         |
|         |         | to be   |         | s-macro |         |         |
|         |         | invalid |         | .aui-   |         |         |
|         |         |         |         | lozenge |         |         |
|         |         |         |         | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-35 |         | Edit    | A       | [PASS]  |         |         |
|         |         | name    | notif   | {.statu |         |         |
|         |         | (valid  | ication | s-macro |         |         |
|         |         | input   | saying  | .aui-   |         |         |
|         |         | name)   | contact | lozenge |         |         |
|         |         | and     | updated | .aui-lo |         |         |
|         |         | address | suc     | zenge-s |         |         |
|         |         | (valid  | cessful | uccess} |         |         |
|         |         | input   | is      |         |         |         |
|         |         | a       | shown   |         |         |         |
|         |         | ddress) |         |         |         |         |
|         |         | and     |         |         |         |         |
|         |         | save    |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-36 | Remove  | Click   | Prompts | [PASS]  |         |         |
|         | address | on      | for     | {.statu |         |         |
|         |         | remove  | user    | s-macro |         |         |
|         |         | address | confi   | .aui-   |         |         |
|         |         |         | rmation | lozenge |         |         |
|         |         |         |         | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-37 |         | Click   | Contact | [PASS]  |         |         |
|         |         | remove  | is      | {.statu |         |         |
|         |         | contact | removed | s-macro |         |         |
|         |         |         | from    | .aui-   |         |         |
|         |         |         | address | lozenge |         |         |
|         |         |         | book    | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
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
| Menu-40 | Sign    | Click   | Go back | [PASS]  |         |         |
|         | Out     | on      | to Sign | {.statu |         |         |
|         |         | "Sign   | In page | s-macro |         |         |
|         |         | Out"    |         | .aui-   |         |         |
|         |         | button  |         | lozenge |         |         |
|         |         |         |         | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
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
| 1.1.7-1 |         |         |         |         |         |         |
| -Transf |         |         |         |         |         |         |
| er(NewD |         |         |         |         |         |         |
| esign)} |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| **Test  | **Test  | **Test  | **E     | **S     | **R     | **Auto  |
| Case    | Scen    | steps** | xpected | tatus** | emark** | mated** |
| ID**    | arios** |         | r       |         |         |         |
|         |         |         | esult** |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-1  | Sender  | Click   | A drop  | [PASS]  |         |         |
|         | account | t       | down    | {.statu |         |         |
|         | (T      | ransfer | list of | s-macro |         |         |
|         | ransfer | from    | a       | .aui-   |         |         |
|         | from)   | account | ccounts | lozenge |         |         |
|         |         |         | av      | .aui-lo |         |         |
|         |         |         | ailable | zenge-s |         |         |
|         |         |         | in      | uccess} |         |         |
|         |         |         | wallet  |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-2  |         | Select  | Sender  | [PASS]  |         |         |
|         |         | another | account | {.statu |         |         |
|         |         | account | is      | s-macro |         |         |
|         |         | from    | changed | .aui-   |         |         |
|         |         | drop    |         | lozenge |         |         |
|         |         | down    |         | .aui-lo |         |         |
|         |         | list    |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-3  | R       | Enter   | Icon    | [PASS]  |         |         |
|         | eceiver | invalid | saying  | {.statu |         |         |
|         | account | wallet  | invalid | s-macro |         |         |
|         | (T      | address |         | .aui-   |         |         |
|         | ransfer |         |         | lozenge |         |         |
|         | to)     |         |         | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-4  |         | Click   | A drop  | [PASS]  |         |         |
|         |         | select  | down    | {.statu |         |         |
|         |         | contact | list of | s-macro |         |         |
|         |         |         | c       | .aui-   |         |         |
|         |         |         | ontacts | lozenge |         |         |
|         |         |         | from    | .aui-lo |         |         |
|         |         |         | address | zenge-s |         |         |
|         |         |         | book    | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-5  | T       | Leave   | Could   | [PASS]  |         |         |
|         | ransfer | t       | not     | {.statu |         |         |
|         | amount  | ransfer | proceed | s-macro |         |         |
|         |         | amount  | and     | .aui-   |         |         |
|         |         | as 0    | t       | lozenge |         |         |
|         |         |         | ransfer | .aui-lo |         |         |
|         |         |         | button  | zenge-s |         |         |
|         |         |         | is      | uccess} |         |         |
|         |         |         | d       |         |         |         |
|         |         |         | isabled |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-6  | Message | Enter   | Tran    | [PASS]  |         |         |
|         |         | random  | saction | {.statu |         |         |
|         |         | m       | Fee     | s-macro |         |         |
|         |         | essages | in      | .aui-   |         |         |
|         |         |         | creases | lozenge |         |         |
|         |         |         | as      | .aui-lo |         |         |
|         |         |         | message | zenge-s |         |         |
|         |         |         | size    | uccess} |         |         |
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
|         |         |         |         |         | 9911705 |         |
|         |         |         |         |         | 7_5b142 |         |
|         |         |         |         |         | d79091e |         |
|         |         |         |         |         | 9f17116 |         |
|         |         |         |         |         | 363a5"} |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-8  | P       | Leave   | Shows   | [PASS]  |         |         |
|         | assword | p       | an      | {.statu |         |         |
|         |         | assword | error   | s-macro |         |         |
|         |         | field   | saying  | .aui-   |         |         |
|         |         | empty   | to      | lozenge |         |         |
|         |         |         | enter   | .aui-lo |         |         |
|         |         |         | wallet  | zenge-s |         |         |
|         |         |         | p       | uccess} |         |         |
|         |         |         | assword |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-9  | T       | Enter   | T       | [PASS]  |         |         |
|         | ransfer | valid   | ransfer | {.statu |         |         |
|         | xpx     | wallet  | tran    | s-macro |         |         |
|         |         | a       | saction | .aui-   |         |         |
|         |         | ddress, | is      | lozenge |         |         |
|         |         | valid   | succe   | .aui-lo |         |         |
|         |         | t       | ssfully | zenge-s |         |         |
|         |         | ransfer | created | uccess} |         |         |
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
| TSFR-10 |         | Enter   | Shows   | [PASS]  |         |         |
|         |         | valid   | an      | {.statu |         |         |
|         |         | wallet  | error   | s-macro |         |         |
|         |         | a       | saying  | .aui-   |         |         |
|         |         | ddress, | wallet  | lozenge |         |         |
|         |         | valid   | p       | .aui-lo |         |         |
|         |         | t       | assword | zenge-s |         |         |
|         |         | ransfer | is      | uccess} |         |         |
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
| TSFR-11 | T       | Click   | If      | [PASS]  |         |         |
|         | ransfer | to add  | amount  | {.statu |         |         |
|         | Asset   | asset   | of      | s-macro |         |         |
|         |         | for     | asset   | .aui-   |         |         |
|         |         | t       | entered | lozenge |         |         |
|         |         | ransfer | exceeds | .aui-lo |         |         |
|         |         |         | asset   | zenge-s |         |         |
|         |         |         | b       | uccess} |         |         |
|         |         |         | alance, |         |         |         |
|         |         |         | an      |         |         |         |
|         |         |         | error   |         |         |         |
|         |         |         | is      |         |         |         |
|         |         |         | shown   |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-12 | Cancel  | Click   | User is | [PASS]  |         |         |
|         |         | on      | d       | {.statu |         |         |
|         |         | cancel  | irected | s-macro |         |         |
|         |         |         | back to | .aui-   |         |         |
|         |         |         | home    | lozenge |         |         |
|         |         |         | page    | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-13 | Eye     | Click   | Sh      | [PASS]  |         |         |
|         | icon    | on eye  | ow/hide | {.statu |         |         |
|         |         | icon    | p       | s-macro |         |         |
|         |         | beside  | assword | .aui-   |         |         |
|         |         | p       |         | lozenge |         |         |
|         |         | assword |         | .aui-lo |         |         |
|         |         | field   |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
:::

::: table-wrap
+---------+---------+---------+---------+---------+---------+---------+
| ## Acco |         |         |         |         |         |         |
| unts {# |         |         |         |         |         |         |
| TestRep |         |         |         |         |         |         |
| ort-1.1 |         |         |         |         |         |         |
| .7-1-Ac |         |         |         |         |         |         |
| counts} |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| **Test  | **Test  | **Test  | **E     | **S     | **R     | **Auto  |
| Case    | Scen    | steps** | xpected | tatus** | emark** | mated** |
| ID**    | arios** |         | r       |         |         |         |
|         |         |         | esult** |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCTS-1 | Create  | Click   | Go to   | [PASS]  |         |         |
|         | a New   | "Create | "       | {.statu |         |         |
|         | Account | New     | Account | s-macro |         |         |
|         |         | A       | \>      | .aui-   |         |         |
|         |         | ccount" | +Create | lozenge |         |         |
|         |         |         | New     | .aui-lo |         |         |
|         |         |         | Account | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCTS-2 | Account | Click   | Go to   | [PASS]  |         |         |
|         | Details | on any  | "       | {.statu |         |         |
|         |         | account | Account | s-macro |         |         |
|         |         | under   | \>      | .aui-   |         |         |
|         |         | A       | D       | lozenge |         |         |
|         |         | ccounts | etails" | .aui-lo |         |         |
|         |         | \>      | page    | zenge-s |         |         |
|         |         | Details |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCTS-3 | Make as | Click   | Account | [PASS]  |         |         |
|         | Default | on      | Av      | {.statu |         |         |
|         |         | default | ailable | s-macro |         |         |
|         |         | button  | pop up  | .aui-   |         |         |
|         |         | beside  | will    | lozenge |         |         |
|         |         | DEFAULT | show    | .aui-lo |         |         |
|         |         | ACCOUNT | up,     | zenge-s |         |         |
|         |         |         | user    | uccess} |         |         |
|         |         |         | can     |         |         |         |
|         |         |         | select  |         |         |         |
|         |         |         | which   |         |         |         |
|         |         |         | account |         |         |         |
|         |         |         | to be   |         |         |         |
|         |         |         | chosen  |         |         |         |
|         |         |         | as      |         |         |         |
|         |         |         | default |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCTS-4 | Export  | Click   | Account | [PASS]  |         |         |
|         | Account | on      | will be | {.statu |         |         |
|         |         | export  | e       | s-macro |         |         |
|         |         | button  | xported | .aui-   |         |         |
|         |         | under   | to      | lozenge |         |         |
|         |         | wallets | local   | .aui-lo |         |         |
|         |         |         | machine | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCTS-5 | Delete  | Click   | Prompt  | [PASS]  |         |         |
|         | an      | on      | for     | {.statu |         |         |
|         | Account | "Delete | confi   | s-macro |         |         |
|         |         | This    | rmation | .aui-   |         |         |
|         |         | A       | to      | lozenge |         |         |
|         |         | ccount" | delete  | .aui-lo |         |         |
|         |         | button  | the     | zenge-s |         |         |
|         |         |         | a       | uccess} |         |         |
|         |         |         | ccount, |         |         |         |
|         |         |         | p       |         |         |         |
|         |         |         | assword |         |         |         |
|         |         |         | is      |         |         |         |
|         |         |         | r       |         |         |         |
|         |         |         | equired |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCTS-6 |         | Enter   | Account | [PASS]  |         |         |
|         |         | Correct | succe   | {.statu |         |         |
|         |         | Account | ssfully | s-macro |         |         |
|         |         | Pas     | removed | .aui-   |         |         |
|         |         | sword,\ | with a  | lozenge |         |         |
|         |         | Click   | notif   | .aui-lo |         |         |
|         |         | "       | ication | zenge-s |         |         |
|         |         | Confirm | p       | uccess} |         |         |
|         |         | De      | rompted |         |         |         |
|         |         | letion" | for     |         |         |         |
|         |         |         | user    |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCTS-7 |         | Enter   | User is | [PASS]  |         |         |
|         |         | Correct | d       | {.statu |         |         |
|         |         | Account | irected | s-macro |         |         |
|         |         | Pas     | back to | .aui-   |         |         |
|         |         | sword,\ | account | lozenge |         |         |
|         |         | Click   | details | .aui-lo |         |         |
|         |         | "       | page    | zenge-s |         |         |
|         |         | Cancel" |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCTS-8 |         | Enter   | An      | [PASS]  |         |         |
|         |         | In      | error   | {.statu |         |         |
|         |         | correct | is      | s-macro |         |         |
|         |         | Account | shown   | .aui-   |         |         |
|         |         | Pas     |         | lozenge |         |         |
|         |         | sword,\ |         | .aui-lo |         |         |
|         |         | Click   |         | zenge-s |         |         |
|         |         | "       |         | uccess} |         |         |
|         |         | Confirm |         |         |         |         |
|         |         | De      |         |         |         |         |
|         |         | letion" |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCTS-9 | Eye     | Click   | Sh      | [PASS]  |         |         |
|         | icon    | on      | ow/hide | {.statu |         |         |
|         |         | p       | p       | s-macro |         |         |
|         |         | assword | assword | .aui-   |         |         |
|         |         | eye     |         | lozenge |         |         |
|         |         | icon    |         | .aui-lo |         |         |
|         |         | when    |         | zenge-s |         |         |
|         |         | d       |         | uccess} |         |         |
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
| -1.1.7- |         |         |         |         |         |         |
| 1-Selec |         |         |         |         |         |         |
| tCreati |         |         |         |         |         |         |
| onType} |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| N       | Create  | Click   | Go to   | [PASS]  |         |         |
| EWACC-1 | New     | on      | "Create | {.statu |         |         |
|         |         | "Create | New     | s-macro |         |         |
|         |         | New"    | A       | .aui-   |         |         |
|         |         | button  | ccount" | lozenge |         |         |
|         |         |         | Page    | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| N       | From a  | Click   | Go to   | [PASS]  |         |         |
| EWACC-2 | Private | on      | "Create | {.statu |         |         |
|         | Key     | "From a | New     | s-macro |         |         |
|         |         | Private | Account | .aui-   |         |         |
|         |         | Key"    | From    | lozenge |         |         |
|         |         | button  | Private | .aui-lo |         |         |
|         |         |         | Key"    | zenge-s |         |         |
|         |         |         | Page    | uccess} |         |         |
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
| -1.1.7- |         |         |         |         |         |         |
| 1-Creat |         |         |         |         |         |         |
| eaNewAc |         |         |         |         |         |         |
| countin |         |         |         |         |         |         |
| thesame |         |         |         |         |         |         |
| Wallet} |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| N       | Create  | Cu      | Go to   | [PASS]  |         |         |
| EWACC-3 | a New   | rrently | "Select | {.statu |         |         |
|         | Account | in      | C       | s-macro |         |         |
|         |         | "Create | reation | .aui-   |         |         |
|         |         | New     | Type"   | lozenge |         |         |
|         |         | A       |         | .aui-lo |         |         |
|         |         | ccount" |         | zenge-s |         |         |
|         |         | page    |         | uccess} |         |         |
|         |         | and     |         |         |         |         |
|         |         | click   |         |         |         |         |
|         |         | "Back"  |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| N       |         | Leave   | Show a  | [PASS]  |         |         |
| EWACC-4 |         | account | message | {.statu |         |         |
|         |         | name    | "Enter  | s-macro |         |         |
|         |         | empty   | Account | .aui-   |         |         |
|         |         |         | Name"   | lozenge |         |         |
|         |         |         |         | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| N       |         | Enter   | Show a  | [PASS]  |         |         |
| EWACC-5 |         | Account | message | {.statu |         |         |
|         |         | Name,\  | "min    | s-macro |         |         |
|         |         | Leave   | length  | .aui-   |         |         |
|         |         | p       | 8",     | lozenge |         |         |
|         |         | assword | unable  | .aui-lo |         |         |
|         |         | field   | to      | zenge-s |         |         |
|         |         | empty   | create  | uccess} |         |         |
|         |         |         | account |         |         |         |
|         |         |         | (create |         |         |         |
|         |         |         | button  |         |         |         |
|         |         |         | di      |         |         |         |
|         |         |         | sabled) |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| N       |         | Enter   | Show a  | [PASS]  |         |         |
| EWACC-6 |         | Account | message | {.statu |         |         |
|         |         | Name,\  | "P      | s-macro |         |         |
|         |         | Enter   | assword | .aui-   |         |         |
|         |         | in      | for     | lozenge |         |         |
|         |         | correct | wallet  | .aui-lo |         |         |
|         |         | Wallet  | \<name  | zenge-s |         |         |
|         |         | Pa      | of      | uccess} |         |         |
|         |         | ssword\ | w       |         |         |         |
|         |         | Click   | allet\> |         |         |         |
|         |         | "       | is      |         |         |         |
|         |         | Create" | i       |         |         |         |
|         |         |         | nvalid" |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| N       |         | Enter   | Send a  | [PASS]  |         |         |
| EWACC-7 |         | Account | confi   | {.statu |         |         |
|         |         | Name,\  | rmation | s-macro |         |         |
|         |         | Enter   | message | .aui-   |         |         |
|         |         | Correct | and     | lozenge |         |         |
|         |         | Wallet  | create  | .aui-lo |         |         |
|         |         | Pa      | the     | zenge-s |         |         |
|         |         | ssword\ | account | uccess} |         |         |
|         |         | Click   |         |         |         |         |
|         |         | "       |         |         |         |         |
|         |         | Create" |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| N       | Eye     | Click   | Sh      | [PASS]  |         |         |
| EWACC-8 | icon    | on      | ow/hide | {.statu |         |         |
|         |         | "Pa     | p       | s-macro |         |         |
|         |         | ssword" | assword | .aui-   |         |         |
|         |         | eye     |         | lozenge |         |         |
|         |         | icon    |         | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
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
| -1.1.7- |         |         |         |         |         |         |
| 1-Creat |         |         |         |         |         |         |
| eaNewAc |         |         |         |         |         |         |
| countfr |         |         |         |         |         |         |
| omPriva |         |         |         |         |         |         |
| teKeyin |         |         |         |         |         |         |
| thesame |         |         |         |         |         |         |
| Wallet} |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| N       | Create  | Cu      | Go to   | [PASS]  |         |         |
| EWACC-9 | a New   | rrently | "Select | {.statu |         |         |
|         | Account | in      | C       | s-macro |         |         |
|         | from    | "Create | reation | .aui-   |         |         |
|         | Private | New     | Type"   | lozenge |         |         |
|         | Key     | Account |         | .aui-lo |         |         |
|         |         | From    |         | zenge-s |         |         |
|         |         | Private |         | uccess} |         |         |
|         |         | Key"    |         |         |         |         |
|         |         | page    |         |         |         |         |
|         |         | and     |         |         |         |         |
|         |         | click   |         |         |         |         |
|         |         | "Back"  |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Leave   | Show a  | [PASS]  |         |         |
| WACC-10 |         | Private | message | {.statu |         |         |
|         |         | Key     | "       | s-macro |         |         |
|         |         | empty   | Invalid | .aui-   |         |         |
|         |         |         | Private | lozenge |         |         |
|         |         |         | Key"    | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Enter   | Show a  | [PASS]  |         |         |
| WACC-11 |         | Private | message | {.statu |         |         |
|         |         | Key,\   | "Enter  | s-macro |         |         |
|         |         | Leave   | Wallet  | .aui-   |         |         |
|         |         | Account | Name"   | lozenge |         |         |
|         |         | Name    |         | .aui-lo |         |         |
|         |         | empty   |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Enter   | Show a  | [PASS]  |         |         |
| WACC-12 |         | Private | message | {.statu |         |         |
|         |         | Key,\   | "p      | s-macro |         |         |
|         |         | Enter   | assword | .aui-   |         |         |
|         |         | Account | is      | lozenge |         |         |
|         |         | Name,\  | req     | .aui-lo |         |         |
|         |         | Leave   | uired", | zenge-s |         |         |
|         |         | p       | unable  | uccess} |         |         |
|         |         | assword | to      |         |         |         |
|         |         | field   | create  |         |         |         |
|         |         | empty   | account |         |         |         |
|         |         |         | (create |         |         |         |
|         |         |         | button  |         |         |         |
|         |         |         | di      |         |         |         |
|         |         |         | sabled) |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Enter   | Show a  | [PASS]  |         |         |
| WACC-13 |         | Private | message | {.statu |         |         |
|         |         | Key,\   | "P      | s-macro |         |         |
|         |         | Enter   | assword | .aui-   |         |         |
|         |         | Account | for     | lozenge |         |         |
|         |         | Name,\  | wallet  | .aui-lo |         |         |
|         |         | Enter   | \<name  | zenge-s |         |         |
|         |         | in      | of      | uccess} |         |         |
|         |         | correct | w       |         |         |         |
|         |         | wallet  | allet\> |         |         |         |
|         |         | pa      | is      |         |         |         |
|         |         | ssword\ | i       |         |         |         |
|         |         | Click   | nvalid" |         |         |         |
|         |         | "       |         |         |         |         |
|         |         | Create" |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Enter   | Send a  | [PASS]  |         |         |
| WACC-14 |         | Private | confi   | {.statu |         |         |
|         |         | Key,\   | rmation | s-macro |         |         |
|         |         | Enter   | message | .aui-   |         |         |
|         |         | Account | and     | lozenge |         |         |
|         |         | Name,\  | create  | .aui-lo |         |         |
|         |         | Enter   | the     | zenge-s |         |         |
|         |         | correct | account | uccess} |         |         |
|         |         | wallet  |         |         |         |         |
|         |         | pa      |         |         |         |         |
|         |         | ssword\ |         |         |         |         |
|         |         | Click   |         |         |         |         |
|         |         | "       |         |         |         |         |
|         |         | Create" |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      | Eye     | Click   | Sh      | [PASS]  |         |         |
| WACC-15 | icon    | on      | ow/hide | {.statu |         |         |
|         |         | "Pa     | p       | s-macro |         |         |
|         |         | ssword" | assword | .aui-   |         |         |
|         |         | eye     |         | lozenge |         |         |
|         |         | icon    |         | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ##      |         |         |         |         |         |         |
| # Edit  |         |         |         |         |         |         |
| an exis |         |         |         |         |         |         |
| ting Ac |         |         |         |         |         |         |
| count { |         |         |         |         |         |         |
| #TestRe |         |         |         |         |         |         |
| port-1. |         |         |         |         |         |         |
| 1.7-1-E |         |         |         |         |         |         |
| ditanex |         |         |         |         |         |         |
| istingA |         |         |         |         |         |         |
| ccount} |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| #### De |         |         |         |         |         |         |
| tails { |         |         |         |         |         |         |
| #TestRe |         |         |         |         |         |         |
| port-1. |         |         |         |         |         |         |
| 1.7-1-D |         |         |         |         |         |         |
| etails} |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCDE   | Change  | Click   | Account | [PASS]  |         |         |
| TAILS-1 | Account | on      | name    | {.statu |         |         |
|         | Name    | "       | updated | s-macro |         |         |
|         |         | Pencil" | and     | .aui-   |         |         |
|         |         | icon    | re      | lozenge |         |         |
|         |         | beside  | flected | .aui-lo |         |         |
|         |         | Account | under   | zenge-s |         |         |
|         |         | Name,   | the     | uccess} |         |         |
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
| ACCDE   | Copy    | Click   | Wallet  | [PASS]  |         |         |
| TAILS-2 | Wallet  | "Copy"  | Address | {.statu |         |         |
|         | Address | icon    | is      | s-macro |         |         |
|         |         | under   | copied  | .aui-   |         |         |
|         |         | Wallet  | to      | lozenge |         |         |
|         |         | Address | user's  | .aui-lo |         |         |
|         |         |         | cl      | zenge-s |         |         |
|         |         |         | ipboard | uccess} |         |         |
|         |         |         | and a   |         |         |         |
|         |         |         | notif   |         |         |         |
|         |         |         | ication |         |         |         |
|         |         |         | is      |         |         |         |
|         |         |         | shown   |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCDE   | Copy    | Click   | Public  | [PASS]  |         |         |
| TAILS-3 | Public  | "Copy"  | Key is  | {.statu |         |         |
|         | Key     | icon    | copied  | s-macro |         |         |
|         |         | under   | to      | .aui-   |         |         |
|         |         | Public  | user's  | lozenge |         |         |
|         |         | Key     | cl      | .aui-lo |         |         |
|         |         |         | ipboard | zenge-s |         |         |
|         |         |         | and a   | uccess} |         |         |
|         |         |         | notif   |         |         |         |
|         |         |         | ication |         |         |         |
|         |         |         | is      |         |         |         |
|         |         |         | shown   |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCDE   | Show    | Click   | Prompt  | [PASS]  |         |         |
| TAILS-4 | Private | on      | for     | {.statu |         |         |
|         | Key     | "       | user to | s-macro |         |         |
|         |         | Private | enter   | .aui-   |         |         |
|         |         | Key"    | p       | lozenge |         |         |
|         |         | eye     | assword | .aui-lo |         |         |
|         |         | icon\   |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCDE   |         | Enter   | Private | [PASS]  |         |         |
| TAILS-5 |         | correct | Key is  | {.statu |         |         |
|         |         | wallet  | visible | s-macro |         |         |
|         |         | pa      | and     | .aui-   |         |         |
|         |         | ssword\ | allows  | lozenge |         |         |
|         |         | Click   | user to | .aui-lo |         |         |
|         |         | "C      | copy it | zenge-s |         |         |
|         |         | onfirm" |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCDE   |         | Enter   | Go back | [PASS]  |         |         |
| TAILS-6 |         | correct | to      | {.statu |         |         |
|         |         | wallet  | Account | s-macro |         |         |
|         |         | pa      | Details | .aui-   |         |         |
|         |         | ssword\ | page    | lozenge |         |         |
|         |         | Click   |         | .aui-lo |         |         |
|         |         | "       |         | zenge-s |         |         |
|         |         | Cancel" |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCDE   |         | Enter   | Show a  | [PASS]  |         |         |
| TAILS-7 |         | in      | message | {.statu |         |         |
|         |         | correct | "Wallet | s-macro |         |         |
|         |         | wallet  | p       | .aui-   |         |         |
|         |         | pa      | assword | lozenge |         |         |
|         |         | ssword\ | is      | .aui-lo |         |         |
|         |         | Click   | inc     | zenge-s |         |         |
|         |         | "C      | orrect" | uccess} |         |         |
|         |         | onfirm" |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCDE   |         | Enter   | Show a  | [PASS]  |         |         |
| TAILS-8 |         | blank   | message | {.statu |         |         |
|         |         | wallet  | "P      | s-macro |         |         |
|         |         | pa      | assword | .aui-   |         |         |
|         |         | ssword\ | is      | lozenge |         |         |
|         |         | Click   | re      | .aui-lo |         |         |
|         |         | "C      | quired" | zenge-s |         |         |
|         |         | onfirm" |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCDE   | Copy    | Click   | Private | [PASS]  |         |         |
| TAILS-9 | Private | "Copy"  | Key is  | {.statu |         |         |
|         | Key     | icon    | copied  | s-macro |         |         |
|         |         | under   | to      | .aui-   |         |         |
|         |         | Private | user's  | lozenge |         |         |
|         |         | Key     | cl      | .aui-lo |         |         |
|         |         | after   | ipboard | zenge-s |         |         |
|         |         | it is   | and a   | uccess} |         |         |
|         |         | shown   | notif   |         |         |         |
|         |         |         | ication |         |         |         |
|         |         |         | is      |         |         |         |
|         |         |         | shown   |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCDET  | D       | Click   | Prompt  | [PASS]  |         |         |
| AILS-10 | ownload | on      | for     | {.statu |         |         |
|         | Wallet  | "D      | user to | s-macro |         |         |
|         | Paper   | ownload | enter   | .aui-   |         |         |
|         |         | Wallet  | wallet  | lozenge |         |         |
|         |         | Paper"  | p       | .aui-lo |         |         |
|         |         | button  | assword | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
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
| ACCDET  |         | Enter   | Go back | [PASS]  |         |         |
| AILS-12 |         | correct | to      | {.statu |         |         |
|         |         | wallet  | Account | s-macro |         |         |
|         |         | pa      | Details | .aui-   |         |         |
|         |         | ssword\ | page    | lozenge |         |         |
|         |         | Click   |         | .aui-lo |         |         |
|         |         | "       |         | zenge-s |         |         |
|         |         | Cancel" |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCDET  |         | Enter   | Show a  | [PASS]  |         |         |
| AILS-13 |         | in      | message | {.statu |         |         |
|         |         | correct | "Wallet | s-macro |         |         |
|         |         | wallet  | p       | .aui-   |         |         |
|         |         | pa      | assword | lozenge |         |         |
|         |         | ssword\ | is      | .aui-lo |         |         |
|         |         | Click   | inc     | zenge-s |         |         |
|         |         | "C      | orrect" | uccess} |         |         |
|         |         | onfirm" |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCDET  |         | Enter   | Show a  | [PASS]  |         |         |
| AILS-14 |         | blank   | message | {.statu |         |         |
|         |         | wallet  | "P      | s-macro |         |         |
|         |         | pa      | assword | .aui-   |         |         |
|         |         | ssword\ | is      | lozenge |         |         |
|         |         | Click   | re      | .aui-lo |         |         |
|         |         | "C      | quired" | zenge-s |         |         |
|         |         | onfirm" |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCDET  | Eye     | Click   | Sh      | [PASS]  |         |         |
| AILS-15 | icon    | on      | ow/hide | {.statu |         |         |
|         |         | p       | p       | s-macro |         |         |
|         |         | assword | assword | .aui-   |         |         |
|         |         | eye     |         | lozenge |         |         |
|         |         | icon    |         | .aui-lo |         |         |
|         |         | when    |         | zenge-s |         |         |
|         |         | e       |         | uccess} |         |         |
|         |         | ntering |         |         |         |         |
|         |         | wallet  |         |         |         |         |
|         |         | p       |         |         |         |         |
|         |         | assword |         |         |         |         |
|         |         | to show |         |         |         |         |
|         |         | private |         |         |         |         |
|         |         | key     |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCDET  |         | Click   | Hide    | [PASS]  |         |         |
| AILS-16 |         | on hide | private | {.statu |         |         |
|         |         | private | key     | s-macro |         |         |
|         |         | key eye |         | .aui-   |         |         |
|         |         | icon to |         | lozenge |         |         |
|         |         | mask it |         | .aui-lo |         |         |
|         |         | again   |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCDET  | D       | Go to   | Account | [PASS]  |         |         |
| AILS-17 | elegate | "A      | is      | {.statu |         |         |
|         |         | ccounts | linked  | s-macro |         |         |
|         |         | \>      | to a    | .aui-   |         |         |
|         |         | Del     | de      | lozenge |         |         |
|         |         | egate"\ | legated | .aui-lo |         |         |
|         |         | Select  | a       | zenge-s |         |         |
|         |         | a       | ccount\ | uccess} |         |         |
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
| ACCDET  |         | Click   | De      | [PASS]  |         |         |
| AILS-18 |         | "Save   | legated | {.statu |         |         |
|         |         | as      | ac      | s-macro |         |         |
|         |         | Wallet  | count's | .aui-   |         |         |
|         |         | Paper"  | wallet  | lozenge |         |         |
|         |         | button  | paper   | .aui-lo |         |         |
|         |         |         | dow     | zenge-s |         |         |
|         |         |         | nloaded | uccess} |         |         |
|         |         |         | to      |         |         |         |
|         |         |         | user's  |         |         |         |
|         |         |         | local   |         |         |         |
|         |         |         | machine |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCDET  |         | Click   | Go back | [PASS]  |         |         |
| AILS-19 |         | "C      | to      | {.statu |         |         |
|         |         | ontinue | A       | s-macro |         |         |
|         |         |         | ccounts | .aui-   |         |         |
|         |         |         | \> View | lozenge |         |         |
|         |         |         | All     | .aui-lo |         |         |
|         |         |         | page    | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ### Con |         |         |         |         |         |         |
| vert to |         |         |         |         |         |         |
|  Multis |         |         |         |         |         |         |
| ig {#Te |         |         |         |         |         |         |
| stRepor |         |         |         |         |         |         |
| t-1.1.7 |         |         |         |         |         |         |
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
| 1.1.7-1 |         |         |         |         |         |         |
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
| .7-1-Outg |           |           |           |           |   |   |
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

## Services {#TestReport-1.1.7-1-Services}

### Namespaces {#TestReport-1.1.7-1-Namespaces}

#### Register {#TestReport-1.1.7-1-Register style="margin-left: 30.0px;"}

#### Extend Duration {#TestReport-1.1.7-1-ExtendDuration style="margin-left: 30.0px;"}

### Assets {#TestReport-1.1.7-1-Assets}

#### Create {#TestReport-1.1.7-1-Create style="margin-left: 30.0px;"}

#### Modify Supply {#TestReport-1.1.7-1-ModifySupply style="margin-left: 30.0px;"}

#### Link to Namespaces {#TestReport-1.1.7-1-LinktoNamespaces style="margin-left: 30.0px;"}

### Swap {#TestReport-1.1.7-1-Swap}

#### NIS1 {#TestReport-1.1.7-1-NIS1 style="margin-left: 30.0px;"}

#### ETH {#TestReport-1.1.7-1-ETH style="margin-left: 30.0px;"}

#### BSC {#TestReport-1.1.7-1-BSC style="margin-left: 30.0px;"}

### Address Book {#TestReport-1.1.7-1-AddressBook}

#### List {#TestReport-1.1.7-1-List style="margin-left: 30.0px;"}

#### Add Contacts {#TestReport-1.1.7-1-AddContacts style="margin-left: 30.0px;"}

### Wallets {#TestReport-1.1.7-1-Wallets}

#### Change Password {#TestReport-1.1.7-1-ChangePassword style="margin-left: 30.0px;"}

#### Export {#TestReport-1.1.7-1-Export style="margin-left: 30.0px;"}

#### Delete {#TestReport-1.1.7-1-Delete style="margin-left: 30.0px;"}

### Voting {#TestReport-1.1.7-1-Voting}

#### Create Poll {#TestReport-1.1.7-1-CreatePoll style="margin-left: 30.0px;"}

#### Vote {#TestReport-1.1.7-1-Vote style="margin-left: 30.0px;"}

#### View Results {#TestReport-1.1.7-1-ViewResults style="margin-left: 30.0px;"}

### Storage {#TestReport-1.1.7-1-Storage}

#### Files {#TestReport-1.1.7-1-Files style="margin-left: 30.0px;"}

#### Upload File {#TestReport-1.1.7-1-UploadFile style="margin-left: 30.0px;"}

#### Send/Share {#TestReport-1.1.7-1-Send/Share style="margin-left: 30.0px;"}

### Sirius Gift {#TestReport-1.1.7-1-SiriusGift}

#### Create {#TestReport-1.1.7-1-Create.1 style="margin-left: 30.0px;"}

#### Redeem {#TestReport-1.1.7-1-Redeem style="margin-left: 30.0px;"}

### Aggregate Transactions {#TestReport-1.1.7-1-AggregateTransactions}

#### Complete {#TestReport-1.1.7-1-Complete style="margin-left: 30.0px;"}

#### Bonded {#TestReport-1.1.7-1-Bonded style="margin-left: 30.0px;"}
:::

::: {.pageSection .group}
::: pageSectionHeader
## Attachments: {#attachments .pageSectionTitle}
:::

::: {.greybox align="left"}
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2499117057/2499117071)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[b6Y7vdCjGYj4Iz0F_WS65i2cmIOlSUT86qa6i_8b-nI5nMCdfPd8pzyZ7F00oJUCaExJm6trTRKlkKGVJ7Sk77IHaRM8J3xiPRDc7QBvZKdGSgTdYDf5PENJN1AGkDy16cx3ElRHYzDKpmmMJA](attachments/2499117057/2499117074)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[-bO8lWnCxvS5X986IxWgckBxaJCAbxhYl3-TF3royi6Q4j9TP6fotHOWiQ-il3_ryQNouMJ4csO5ZSgD_ZjKbkejc_edkj4PbVtm6f83nPyVS5LMbxvR1CSNaPwQrwZqw6pPpu1WRhThCx6m3A](attachments/2499117057/2499117077)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[JuJFRQviEuNr-LFhKKtzgok1mpF5HDikOIL1_xWg6aGr2qkQ8QSbxpffBmBBZjHP0mp8bWeQOwXRWRwlDCdz6gs25qus8boYnGvW4GVGSyi0cdVFcdwMCJyRp_oVci2AbNXYamEotatFLomrkg](attachments/2499117057/2499117080)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[image-20220321-013652.png](attachments/2499117057/2499117083.png)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[image-20220321-033506.png](attachments/2499117057/2499117086.png)
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
