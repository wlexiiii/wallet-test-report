::: {#page}
::: {#main .aui-page-panel}
::: {#main-header}
::: {#breadcrumb-section}
1.  [ProximaX Tools](index.html)
2.  [Test Reports](Test-Reports_2443871313.html)
:::

# [ ProximaX Tools : Test Report - 1.2.4 - 1 ]{#title-text} {#title-heading .pagetitle}
:::

::: {#content .view}
::: page-metadata
Created by [ Wen Ching]{.author} on Sep 28, 2022
:::

::: {#main-content .wiki-content .group}
Date: 27/09/2022 - 28/09/2022\
Version: 1.2.4-1\
Test Environment: Version 105.0.5195.127 (Official Build) (64-bit),
Intel(R) Core(TM) i3-4030U CPU @ 1.90GHz 1.90 GHz, 4.00 GB RAM\
Staging Link: [: ProximaX Web Wallet (staging
site)](https://proximax-foundry.github.io/web-wallet-vuejs/#/){.external-link
rel="nofollow"}\
Browser: Google Chrome (Version 105.0(64-bit)\
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

::: {.toc-macro .rbtoc1667370016915}
-   [Main Page](#TestReport-1.2.4-1-MainPage)
    -   [Sign In](#TestReport-1.2.4-1-SignIn)
    -   [Create New Wallet](#TestReport-1.2.4-1-CreateNewWallet)
    -   [Create New Wallet From Private
        Key](#TestReport-1.2.4-1-CreateNewWalletFromPrivateKey)
    -   [Import wallet from .wlt file (Create Wallet from a Wallet
        Backup)](#TestReport-1.2.4-1-Importwalletfrom.wltfile(CreateWalletfromaWalletBackup))
-   [Dashboard](#TestReport-1.2.4-1-Dashboard)
-   [Side Menu Bar (Home
    Page)](#TestReport-1.2.4-1-SideMenuBar(HomePage))
-   [Transfer (New Design)](#TestReport-1.2.4-1-Transfer(NewDesign))
-   [Accounts](#TestReport-1.2.4-1-Accounts)
    -   [Select Creation Type](#TestReport-1.2.4-1-SelectCreationType)
        -   [Create a New Account in the same
            Wallet](#TestReport-1.2.4-1-CreateaNewAccountinthesameWallet)
        -   [Create a New Account from Private Key in the same
            Wallet](#TestReport-1.2.4-1-CreateaNewAccountfromPrivateKeyinthesameWallet)
    -   [Edit an existing
        Account](#TestReport-1.2.4-1-EditanexistingAccount)
        -   [Details](#TestReport-1.2.4-1-Details)
    -   [Convert to Multisig](#TestReport-1.2.4-1-ConverttoMultisig)
    -   [Edit Multisig](#TestReport-1.2.4-1-EditMultisig)
    -   [Edit Namespace](#TestReport-1.2.4-1-EditNamespace)
    -   [Edit Asset](#TestReport-1.2.4-1-EditAsset)
    -   [Outgoing Swap](#TestReport-1.2.4-1-OutgoingSwap)
    -   [Incoming Swap](#TestReport-1.2.4-1-IncomingSwap)
-   [Services](#TestReport-1.2.4-1-Services)
    -   [Swap](#TestReport-1.2.4-1-Swap)
        -   [NIS1](#TestReport-1.2.4-1-NIS1)
        -   [ETH](#TestReport-1.2.4-1-ETH)
        -   [BSC](#TestReport-1.2.4-1-BSC)
    -   [Wallets](#TestReport-1.2.4-1-Wallets)
        -   [Change Password](#TestReport-1.2.4-1-ChangePassword)
    -   [Voting](#TestReport-1.2.4-1-Voting)
        -   [Create Poll](#TestReport-1.2.4-1-CreatePoll)
        -   [Vote](#TestReport-1.2.4-1-Vote)
        -   [View Results](#TestReport-1.2.4-1-ViewResults)
    -   [Storage](#TestReport-1.2.4-1-Storage)
        -   [Files](#TestReport-1.2.4-1-Files)
        -   [Upload File](#TestReport-1.2.4-1-UploadFile)
        -   [Send/Share](#TestReport-1.2.4-1-Send/Share)
    -   [Sirius Gift](#TestReport-1.2.4-1-SiriusGift)
        -   [Create](#TestReport-1.2.4-1-Create)
        -   [Redeem](#TestReport-1.2.4-1-Redeem)
    -   [Aggregate
        Transactions](#TestReport-1.2.4-1-AggregateTransactions)
        -   [Complete](#TestReport-1.2.4-1-Complete)
        -   [Bonded](#TestReport-1.2.4-1-Bonded)
:::

::: {.confluence-information-macro .confluence-information-macro-information}
[]{.aui-icon .aui-icon-small .aui-iconfont-info
.confluence-information-macro-icon}

::: confluence-information-macro-body
Status: [NOT READY]{.status-macro .aui-lozenge} [READY]{.status-macro
.aui-lozenge .aui-lozenge-current} [REMOVED]{.status-macro .aui-lozenge
.aui-lozenge-complete}[PASS]{.status-macro .aui-lozenge
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
| ort-1.2 |         |         |         |         |         |         |
| .4-1-Ma |         |         |         |         |         |         |
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
| .2.4-1- |         |         |         |         |         |         |
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
| S       |         | Place   | Show an | [PASS]  |         |         |
| IGNIN-2 |         | less    | error   | {.statu |         |         |
|         |         | than    | "p      | s-macro |         |         |
|         |         | r       | assword | .aui-   |         |         |
|         |         | equired | is      | lozenge |         |         |
|         |         | values  | re      | .aui-lo |         |         |
|         |         |         | quired" | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
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
| ort-1.2 |         |         |         |         |         |         |
| .4-1-Cr |         |         |         |         |         |         |
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
| ort-1.2 |         |         |         |         |         |         |
| .4-1-Cr |         |         |         |         |         |         |
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
| NE      |         | Set     | N/A     | [PASS]  |         |         |
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
| .2.4-1- |         |         |         |         |         |         |
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
| rt-1.2. |         |         |         |         |         |         |
| 4-1-Das |         |         |         |         |         |         |
| hboard} |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| **Test  | **Test  | **Test  | **E     | **S     | **R     | **Auto  |
| Case    | Scen    | steps** | xpected | tatus** | emark** | mated** |
| ID**    | arios** |         | r       |         |         |         |
|         |         |         | esult** |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-1  | Home    | Click   | Back to | [PASS]  |         |         |
|         |         | "Logo"  | da      | {.statu |         |         |
|         |         | icon    | shboard | s-macro |         |         |
|         |         |         | home    | .aui-   |         |         |
|         |         |         | page    | lozenge |         |         |
|         |         |         |         | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-2  | Beg     | Click   | A list  | [PASS]  |         |         |
|         | inner's | on      | of      | {.statu |         |         |
|         | guide   | q       | b       | s-macro |         |         |
|         |         | uestion | eginner | .aui-   |         |         |
|         |         | mark    | guides  | lozenge |         |         |
|         |         | button  | av      | .aui-lo |         |         |
|         |         |         | ailable | zenge-s |         |         |
|         |         |         | for     | uccess} |         |         |
|         |         |         | user    |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-3  |         | Click   | User    | [PASS]  |         |         |
|         |         | on      | d       | {.statu |         |         |
|         |         | getting | irected | s-macro |         |         |
|         |         | Started | to      | .aui-   |         |         |
|         |         |         | getting | lozenge |         |         |
|         |         |         | started | .aui-lo |         |         |
|         |         |         | page    | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-4  |         | Click   | User    | [PASS]  |         |         |
|         |         | on      | d       | {.statu |         |         |
|         |         | What's  | irected | s-macro |         |         |
|         |         | Sirius  | to      | .aui-   |         |         |
|         |         | Chain   | what's  | lozenge |         |         |
|         |         |         | sirius  | .aui-lo |         |         |
|         |         |         | chain   | zenge-s |         |         |
|         |         |         | page    | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-5  |         | Click   | User    | [PASS]  |         |         |
|         |         | on      | d       | {.statu |         |         |
|         |         | What's  | irected | s-macro |         |         |
|         |         | Na      | to      | .aui-   |         |         |
|         |         | mespace | what's  | lozenge |         |         |
|         |         |         | sirius  | .aui-lo |         |         |
|         |         |         | na      | zenge-s |         |         |
|         |         |         | mespace | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-6  |         | Click   | User    | [PASS]  |         |         |
|         |         | on      | d       | {.statu |         |         |
|         |         | What's  | irected | s-macro |         |         |
|         |         | Asset   | to      | .aui-   |         |         |
|         |         |         | what's  | lozenge |         |         |
|         |         |         | asset   | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
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
| DASH-9  | Act     | Click   | An      | [PASS]  |         |         |
|         | ivities | on      | o       | {.statu |         |         |
|         |         | "Acti   | verview | s-macro |         |         |
|         |         | vities" | of      | .aui-   |         |         |
|         |         | tab     | user's  | lozenge |         |         |
|         |         |         | pending | .aui-lo |         |         |
|         |         |         | tran    | zenge-s |         |         |
|         |         |         | saction | uccess} |         |         |
|         |         |         | and     |         |         |         |
|         |         |         | recent  |         |         |         |
|         |         |         | trans   |         |         |         |
|         |         |         | actions |         |         |         |
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
| DASH-11 | Header  | Click   | Wallet  | [PASS]  |         |         |
|         | com     | on copy | address | {.statu |         |         |
|         | ponents | wallet  | is      | s-macro |         |         |
|         |         | address | copied  | .aui-   |         |         |
|         |         | button  | and a   | lozenge |         |         |
|         |         |         | notif   | .aui-lo |         |         |
|         |         |         | ication | zenge-s |         |         |
|         |         |         | is      | uccess} |         |         |
|         |         |         | shown   |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-12 |         | Click   | User    | [PASS]  |         |         |
|         |         | on      | d       | {.statu |         |         |
|         |         | "Swap"  | irected | s-macro |         |         |
|         |         | button  | to swap | .aui-   |         |         |
|         |         |         | page    | lozenge |         |         |
|         |         |         |         | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-13 |         | Click   | Display | [PASS]  |         |         |
|         |         | on      | QR Code | {.statu |         |         |
|         |         | "Scan   | of      | s-macro |         |         |
|         |         | QR      | wallet  | .aui-   |         |         |
|         |         | Code"   | address | lozenge |         |         |
|         |         | button  |         | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-14 |         | Click   | User    | [PASS]  |         |         |
|         |         | on      | d       | {.statu |         |         |
|         |         | "       | irected | s-macro |         |         |
|         |         | Convert | to      | .aui-   |         |         |
|         |         | to      | m       | lozenge |         |         |
|         |         | Mu      | ultisig | .aui-lo |         |         |
|         |         | ltisig" | page    | zenge-s |         |         |
|         |         | button  |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-15 |         | Click   | User is | [PASS]  |         |         |
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
| 2.4-1-S |         |         |         |         |         |         |
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
|         | Account | "A      | irected | s-macro |         | s-macro |
|         |         | ccount" | to      | .aui-   |         | .aui-   |
|         |         | under   | "Create | lozenge |         | lozenge |
|         |         | "Quick  | New     | .aui-lo |         | .aui-lo |
|         |         | Action" | A       | zenge-s |         | zenge-s |
|         |         |         | ccount" | uccess} |         | uccess} |
|         |         |         | Page    |         |         |         |
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
|         |         |         |         |         | b022_25 |         |
|         |         |         |         |         | 3752119 |         |
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
| MENU-7  |         | Enter   | Na      | [PASS]  |         | [R      |
|         |         | valid   | mespace | {.statu |         | EQUIRES |
|         |         | name,\  | created | s-macro |         | MANUAL  |
|         |         | Enter   | with id | .aui-   |         | T       |
|         |         | d       | and     | lozenge |         | ESTING] |
|         |         | uration | exp     | .aui-lo |         | {.statu |
|         |         | of      | iration | zenge-s |         | s-macro |
|         |         | days,\  | ti      | uccess} |         | .aui-   |
|         |         | Enter   | mestamp |         |         | lozenge |
|         |         | correct |         |         |         | .aui-lo |
|         |         | p       |         |         |         | zenge-c |
|         |         | assword |         |         |         | urrent} |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-8  |         | Enter   | User is | [PASS]  |         |         |
|         |         | valid   | d       | {.statu |         |         |
|         |         | name,\  | irected | s-macro |         |         |
|         |         | Enter   | back to | .aui-   |         |         |
|         |         | d       | da      | lozenge |         |         |
|         |         | uration | shboard | .aui-lo |         |         |
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
|         |         | under   | to a    | .aui-   |         |         |
|         |         | "Quick  | page to | lozenge |         |         |
|         |         | Action" | create  | .aui-lo |         |         |
|         |         |         | asset   | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-12 |         | Leave   | Show an | [PASS]  |         |         |
|         |         | supply, | error   | {.statu |         |         |
|         |         | divis   | to      | s-macro |         |         |
|         |         | ibility | enter   | .aui-   |         |         |
|         |         | and     | wallet  | lozenge |         |         |
|         |         | wallet  | p       | .aui-lo |         |         |
|         |         | p       | assword | zenge-s |         |         |
|         |         | assword |         | uccess} |         |         |
|         |         | empty   |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-13 |         | Enter   | User is | [PASS]  |         |         |
|         |         | amount  | d       | {.statu |         |         |
|         |         | of      | irected | s-macro |         |         |
|         |         | s       | to      | .aui-   |         |         |
|         |         | upply,\ | pending | lozenge |         |         |
|         |         | Enter   | tran    | .aui-lo |         |         |
|         |         | divisib | saction | zenge-s |         |         |
|         |         | ility,\ | page    | uccess} |         |         |
|         |         | Enter   | and     |         |         |         |
|         |         | correct | asset   |         |         |         |
|         |         | wallet  | is      |         |         |         |
|         |         | p       | created |         |         |         |
|         |         | assword | with    |         |         |         |
|         |         |         | its     |         |         |         |
|         |         |         | res     |         |         |         |
|         |         |         | pective |         |         |         |
|         |         |         | id and  |         |         |         |
|         |         |         | details |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-14 |         | Enter   | Show an | [PASS]  |         |         |
|         |         | amount  | error   | {.statu |         |         |
|         |         | of      | saying  | s-macro |         |         |
|         |         | s       | wallet  | .aui-   |         |         |
|         |         | upply,\ | p       | lozenge |         |         |
|         |         | Enter   | assword | .aui-lo |         |         |
|         |         | divisib | is      | zenge-s |         |         |
|         |         | ility,\ | in      | uccess} |         |         |
|         |         | Enter   | correct |         |         |         |
|         |         | wrong   |         |         |         |         |
|         |         | wallet  |         |         |         |         |
|         |         | p       |         |         |         |         |
|         |         | assword |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-15 |         | Enter   | User is | [PASS]  |         |         |
|         |         | amount  | d       | {.statu |         |         |
|         |         | of      | irected | s-macro |         |         |
|         |         | s       | back to | .aui-   |         |         |
|         |         | upply,\ | da      | lozenge |         |         |
|         |         | Enter   | shboard | .aui-lo |         |         |
|         |         | divisib | page    | zenge-s |         |         |
|         |         | ility,\ |         | uccess} |         |         |
|         |         | Enter   |         |         |         |         |
|         |         | wallet  |         |         |         |         |
|         |         | p       |         |         |         |         |
|         |         | assword |         |         |         |         |
|         |         | and     |         |         |         |         |
|         |         | cancel  |         |         |         |         |
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
| MENU-19 |         | Click   | wlt     | [PASS]  |         |         |
|         |         | on      | file    | {.statu |         |         |
|         |         | export  | will be | s-macro |         |         |
|         |         | button  | e       | .aui-   |         |         |
|         |         | under   | xported | lozenge |         |         |
|         |         | wallets | to      | .aui-lo |         |         |
|         |         |         | local   | zenge-s |         |         |
|         |         |         | machine | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-   | A       | Click   | D       | [PASS]  |         |         |
| 20      | ccounts | on      | isplays | {.statu |         |         |
|         |         | "Ac     | an      | s-macro |         |         |
|         |         | counts" | o       | .aui-   |         |         |
|         |         | under   | verview | lozenge |         |         |
|         |         | "Na     | of the  | .aui-lo |         |         |
|         |         | vigate" | user's  | zenge-s |         |         |
|         |         |         | a       | uccess} |         |         |
|         |         |         | ccounts |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-21 |         | Click   | D       | [PASS]  |         |         |
|         |         | on      | isplays | {.statu |         |         |
|         |         | s       | user's  | s-macro |         |         |
|         |         | pecific | account | .aui-   |         |         |
|         |         | account | details | lozenge |         |         |
|         |         |         |         | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-22 |         | Click   | Address | [PASS]  |         |         |
|         |         | copy    | succe   | {.statu |         |         |
|         |         | icon on | ssfully | s-macro |         |         |
|         |         | account | copied  | .aui-   |         |         |
|         |         | address | with    | lozenge |         |         |
|         |         |         | notif   | .aui-lo |         |         |
|         |         |         | ication | zenge-s |         |         |
|         |         |         | p       | uccess} |         |         |
|         |         |         | rompted |         |         |         |
|         |         |         | to user |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-23 |         | Click   | user    | [PASS]  |         |         |
|         |         | on      | d       | {.statu |         |         |
|         |         | "       | irected | s-macro |         |         |
|         |         | +Create | to      | .aui-   |         |         |
|         |         | New     | "Create | lozenge |         |         |
|         |         | A       | New     | .aui-lo |         |         |
|         |         | ccount" | A       | zenge-s |         |         |
|         |         |         | ccount" | uccess} |         |         |
|         |         |         | page    |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-24 | Address | Click   | D       | [PASS]  |         |         |
|         | Book    | on      | isplays | {.statu |         |         |
|         |         | "       | user's  | s-macro |         |         |
|         |         | Address | address | .aui-   |         |         |
|         |         | Book"   | book    | lozenge |         |         |
|         |         | under   | list    | .aui-lo |         |         |
|         |         | "Na     |         | zenge-s |         |         |
|         |         | vigate" |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-25 |         | Click   | User    | [PASS]  |         |         |
|         |         | on      | d       | {.statu |         |         |
|         |         | "+New"  | irected | s-macro |         |         |
|         |         |         | to "Add | .aui-   |         |         |
|         |         |         | New     | lozenge |         |         |
|         |         |         | C       | .aui-lo |         |         |
|         |         |         | ontact" | zenge-s |         |         |
|         |         |         | page    | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-26 |         | Enter   | Shows a | [PASS]  |         |         |
|         |         | valid   | message | {.statu |         |         |
|         |         | ad      | saying  | s-macro |         |         |
|         |         | dress,\ | name is | .aui-   |         |         |
|         |         | Leave   | r       | lozenge |         |         |
|         |         | name    | equired | .aui-lo |         |         |
|         |         | empty   |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-27 |         | Enter   | Show an | [PASS]  |         |         |
|         |         | name,\  | error   | {.statu |         |         |
|         |         | Enter   | (       | s-macro |         |         |
|         |         | invalid | address | .aui-   |         |         |
|         |         | address | is      | lozenge |         |         |
|         |         |         | re      | .aui-lo |         |         |
|         |         |         | quired) | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-28 |         | Enter   | Shows a | [PASS]  |         |         |
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
| MENU-29 |         | Enter   | Shows a | [PASS]  |         |         |
|         |         | an      | message | {.statu |         |         |
|         |         | address | saying  | s-macro |         |         |
|         |         | that    | the     | .aui-   |         |         |
|         |         | already | address | lozenge |         |         |
|         |         | exists  | exists  | .aui-lo |         |         |
|         |         | in the  | in the  | zenge-s |         |         |
|         |         | wallet  | wallet  | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-30 |         | Enter   | New     | [PASS]  |         |         |
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
| MENU-31 | Custom  | Enter   | Enter   | [PASS]  |         |         |
|         |         | name,\  | custom  | {.statu |         |         |
|         |         | Enter   | group   | s-macro |         |         |
|         |         | valid   | name    | .aui-   |         |         |
|         |         | ad      | pop up  | lozenge |         |         |
|         |         | dress,\ | is      | .aui-lo |         |         |
|         |         | Choose  | shown   | zenge-s |         |         |
|         |         | custom  |         | uccess} |         |         |
|         |         | group   |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-32 |         | Enter   | New     | [PASS]  |         |         |
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
| MENU-33 | Edit    | Click   | User    | [PASS]  |         |         |
|         | address | on edit | d       | {.statu |         |         |
|         |         | address | irected | s-macro |         |         |
|         |         |         | to edit | .aui-   |         |         |
|         |         |         | contact | lozenge |         |         |
|         |         |         | page    | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-34 |         | Edit    | Show an | [PASS]  |         |         |
|         |         | name    | error   | {.statu |         |         |
|         |         | field   |         | s-macro |         |         |
|         |         | to be   |         | .aui-   |         |         |
|         |         | empty   |         | lozenge |         |         |
|         |         |         |         | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-35 |         | Edit    | Show an | [PASS]  |         |         |
|         |         | address | error   | {.statu |         |         |
|         |         | to be   |         | s-macro |         |         |
|         |         | invalid |         | .aui-   |         |         |
|         |         |         |         | lozenge |         |         |
|         |         |         |         | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-36 |         | Edit    | A       | [PASS]  |         |         |
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
| MENU-37 | Remove  | Click   | Prompts | [PASS]  |         |         |
|         | address | on      | for     | {.statu |         |         |
|         |         | remove  | user    | s-macro |         |         |
|         |         | address | confi   | .aui-   |         |         |
|         |         |         | rmation | lozenge |         |         |
|         |         |         |         | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-38 |         | Click   | Contact | [PASS]  |         |         |
|         |         | remove  | is      | {.statu |         |         |
|         |         | contact | removed | s-macro |         |         |
|         |         |         | from    | .aui-   |         |         |
|         |         |         | address | lozenge |         |         |
|         |         |         | book    | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-39 | Import  | Click   | Prompts | [PASS]  |         | [R      |
|         | Contact | on      | for     | {.statu |         | EQUIRES |
|         |         | import  | user to | s-macro |         | MANUAL  |
|         |         | tab,    | choose  | .aui-   |         | T       |
|         |         | click   | file to | lozenge |         | ESTING] |
|         |         | import  | add     | .aui-lo |         | {.statu |
|         |         | button  | contact | zenge-s |         | s-macro |
|         |         |         |         | uccess} |         | .aui-   |
|         |         |         |         |         |         | lozenge |
|         |         |         |         |         |         | .aui-lo |
|         |         |         |         |         |         | zenge-c |
|         |         |         |         |         |         | urrent} |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-40 | Export  | Click   | Contact | [PASS]  |         | [R      |
|         | Contact | on      | is      | {.statu |         | EQUIRES |
|         |         | export  | dow     | s-macro |         | MANUAL  |
|         |         | tab,    | nloaded | .aui-   |         | T       |
|         |         | click   | to      | lozenge |         | ESTING] |
|         |         | export  | user's  | .aui-lo |         | {.statu |
|         |         | button  | local   | zenge-s |         | s-macro |
|         |         |         | machine | uccess} |         | .aui-   |
|         |         |         |         |         |         | lozenge |
|         |         |         |         |         |         | .aui-lo |
|         |         |         |         |         |         | zenge-c |
|         |         |         |         |         |         | urrent} |
+---------+---------+---------+---------+---------+---------+---------+
| Menu-41 | Sign    | Click   | Go back | [PASS]  |         |         |
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
| 1.2.4-1 |         |         |         |         |         |         |
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
| TSFR-5  | T       | Leave   | Warning | [PASS]  |         | [YES]   |
|         | ransfer | t       | message | {.statu |         | {.statu |
|         | amount  | ransfer | would   | s-macro |         | s-macro |
|         |         | amount  | appear  | .aui-   |         | .aui-   |
|         |         | as 0    | as "a   | lozenge |         | lozenge |
|         |         |         | confi   | .aui-lo |         | .aui-lo |
|         |         |         | rmation | zenge-s |         | zenge-s |
|         |         |         | for 0   | uccess} |         | uccess} |
|         |         |         | amount" |         |         |         |
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
| TSFR-7  |         | Enter   | P       | [PASS]  |         | [R      |
|         |         | more    | revents | {.statu |         | EQUIRES |
|         |         | than    | input   | s-macro |         | MANUAL  |
|         |         | maximum | upon    | .aui-   |         | T       |
|         |         | of      | r       | lozenge |         | ESTING] |
|         |         | message | eaching | .aui-lo |         | {.statu |
|         |         | limit   | maximum | zenge-s |         | s-macro |
|         |         |         | message | uccess} |         | .aui-   |
|         |         |         | limit   |         |         | lozenge |
|         |         |         |         |         |         | .aui-lo |
|         |         |         |         |         |         | zenge-c |
|         |         |         |         |         |         | urrent} |
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
| ort-1.2 |         |         |         |         |         |         |
| .4-1-Ac |         |         |         |         |         |         |
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
|         |         |         | page    | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| ACCTS-3 | Make as | Click   | Account | [PASS]  |         | [YES]   |
|         | Default | on any  | s       | {.statu |         | {.statu |
|         |         | account | elected | s-macro |         | s-macro |
|         |         | under   | will be | .aui-   |         | .aui-   |
|         |         | A       | change  | lozenge |         | lozenge |
|         |         | ccounts | to      | .aui-lo |         | .aui-lo |
|         |         |         | default | zenge-s |         | zenge-s |
|         |         |         | account | uccess} |         | uccess} |
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
| ACCTS-5 | Delete  | Click   | Prompt  | [R      |         |         |
|         | an      | on      | for     | EMOVED] |         |         |
|         | Account | "Delete | confi   | {.statu |         |         |
|         |         | This    | rmation | s-macro |         |         |
|         |         | A       | to      | .aui-   |         |         |
|         |         | ccount" | delete  | lozenge |         |         |
|         |         | button  | the     | .       |         |         |
|         |         |         | a       | aui-loz |         |         |
|         |         |         | ccount, | enge-co |         |         |
|         |         |         | p       | mplete} |         |         |
|         |         |         | assword |         |         |         |
|         |         |         | is      |         |         |         |
|         |         |         | r       |         |         |         |
|         |         |         | equired |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCTS-6 |         | Enter   | Account | [R      |         |         |
|         |         | Correct | succe   | EMOVED] |         |         |
|         |         | Account | ssfully | {.statu |         |         |
|         |         | Pas     | removed | s-macro |         |         |
|         |         | sword,\ | with a  | .aui-   |         |         |
|         |         | Click   | notif   | lozenge |         |         |
|         |         | "       | ication | .       |         |         |
|         |         | Confirm | p       | aui-loz |         |         |
|         |         | De      | rompted | enge-co |         |         |
|         |         | letion" | for     | mplete} |         |         |
|         |         |         | user    |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCTS-7 |         | Enter   | User is | [R      |         |         |
|         |         | Correct | d       | EMOVED] |         |         |
|         |         | Account | irected | {.statu |         |         |
|         |         | Pas     | back to | s-macro |         |         |
|         |         | sword,\ | account | .aui-   |         |         |
|         |         | Click   | details | lozenge |         |         |
|         |         | "       | page    | .       |         |         |
|         |         | Cancel" |         | aui-loz |         |         |
|         |         |         |         | enge-co |         |         |
|         |         |         |         | mplete} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCTS-8 |         | Enter   | An      | [R      |         |         |
|         |         | In      | error   | EMOVED] |         |         |
|         |         | correct | is      | {.statu |         |         |
|         |         | Account | shown   | s-macro |         |         |
|         |         | Pas     |         | .aui-   |         |         |
|         |         | sword,\ |         | lozenge |         |         |
|         |         | Click   |         | .       |         |         |
|         |         | "       |         | aui-loz |         |         |
|         |         | Confirm |         | enge-co |         |         |
|         |         | De      |         | mplete} |         |         |
|         |         | letion" |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCTS-9 | Eye     | Click   | Sh      | [R      |         |         |
|         | icon    | on      | ow/hide | EMOVED] |         |         |
|         |         | p       | p       | {.statu |         |         |
|         |         | assword | assword | s-macro |         |         |
|         |         | eye     |         | .aui-   |         |         |
|         |         | icon    |         | lozenge |         |         |
|         |         | when    |         | .       |         |         |
|         |         | d       |         | aui-loz |         |         |
|         |         | eleting |         | enge-co |         |         |
|         |         | account |         | mplete} |         |         |
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
| -1.2.4- |         |         |         |         |         |         |
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
| -1.2.4- |         |         |         |         |         |         |
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
|         |         | Name,\  | "P      | s-macro |         |         |
|         |         | Leave   | assword | .aui-   |         |         |
|         |         | p       | is      | lozenge |         |         |
|         |         | assword | req     | .aui-lo |         |         |
|         |         | field   | uired", | zenge-s |         |         |
|         |         | empty   | unable  | uccess} |         |         |
|         |         |         | to      |         |         |         |
|         |         |         | create  |         |         |         |
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
| -1.2.4- |         |         |         |         |         |         |
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
| 2.4-1-E |         |         |         |         |         |         |
| ditanex |         |         |         |         |         |         |
| istingA |         |         |         |         |         |         |
| ccount} |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| #### De |         |         |         |         |         |         |
| tails { |         |         |         |         |         |         |
| #TestRe |         |         |         |         |         |         |
| port-1. |         |         |         |         |         |         |
| 2.4-1-D |         |         |         |         |         |         |
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
|         |         | "C      |         |         |         |         |
|         |         | onfirm" |         |         |         |         |
|         |         | button  |         |         |         |         |
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
| ACCDET  |         | Enter   | User's  | [FAIL]  | [       | [R      |
| AILS-11 |         | correct | wallet  | {.statu | [[]{.a  | EQUIRES |
|         |         | wallet  | paper   | s-macro | ui-icon | MANUAL  |
|         |         | pa      | dow     | .aui-   | .aui-ic | T       |
|         |         | ssword\ | nloaded | lozenge | on-wait | ESTING] |
|         |         | Click   | to      | .aui-   | .issue  | {.statu |
|         |         | "C      | their   | lozenge | -placeh | s-macro |
|         |         | onfirm" | local   | -error} | older}W | .aui-   |
|         |         |         | machine |         | LT-85]( | lozenge |
|         |         |         |         |         | https:/ | .aui-lo |
|         |         |         |         |         | /nemspf | zenge-c |
|         |         |         |         |         | s.atlas | urrent} |
|         |         |         |         |         | sian.ne |         |
|         |         |         |         |         | t/brows |         |
|         |         |         |         |         | e/WLT-8 |         |
|         |         |         |         |         | 5){.jir |         |
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
|         |         |         |         |         | WLT-85" |         |
|         |         |         |         |         | c       |         |
|         |         |         |         |         | lient-i |         |
|         |         |         |         |         | d="SING |         |
|         |         |         |         |         | LE_5581 |         |
|         |         |         |         |         | e30e-87 |         |
|         |         |         |         |         | 6a-3bbe |         |
|         |         |         |         |         | -9902-8 |         |
|         |         |         |         |         | 6eb613c |         |
|         |         |         |         |         | b022_25 |         |
|         |         |         |         |         | 3752119 |         |
|         |         |         |         |         | 7_5b142 |         |
|         |         |         |         |         | d79091e |         |
|         |         |         |         |         | 9f17116 |         |
|         |         |         |         |         | 363a5"} |         |
|         |         |         |         |         |         |         |
|         |         |         |         |         | same    |         |
|         |         |         |         |         | problem |         |
|         |         |         |         |         | (       |         |
|         |         |         |         |         | WLT-85) |         |
|         |         |         |         |         | still   |         |
|         |         |         |         |         | occurs. |         |
|         |         |         |         |         | Paper   |         |
|         |         |         |         |         | wallet  |         |
|         |         |         |         |         | still   |         |
|         |         |         |         |         | d       |         |
|         |         |         |         |         | ownload |         |
|         |         |         |         |         | m       |         |
|         |         |         |         |         | ultiple |         |
|         |         |         |         |         | files.  |         |
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
| ACCDET  | D       | Go to   | Account | [PASS]  |         |         |
| AILS-17 | elegate | "A      | is      | {.statu |         |         |
|         |         | ccounts | linked  | s-macro |         |         |
|         |         | \>      | to a    | .aui-   |         |         |
|         |         | De      | de      | lozenge |         |         |
|         |         | tails\> | legated | .aui-lo |         |         |
|         |         | Linked  | a       | zenge-s |         |         |
|         |         | ac      | ccount\ | uccess} |         |         |
|         |         | count"\ | Public  |         |         |         |
|         |         | Select  | and     |         |         |         |
|         |         | a       | private |         |         |         |
|         |         | linking | keys    |         |         |         |
|         |         | a       | av      |         |         |         |
|         |         | ccount\ | ailable |         |         |         |
|         |         | Account | for     |         |         |         |
|         |         | type as | user to |         |         |         |
|         |         | "New    | store   |         |         |         |
|         |         | A       |         |         |         |         |
|         |         | ccount" |         |         |         |         |
|         |         | or      |         |         |         |         |
|         |         | "From a |         |         |         |         |
|         |         | Private |         |         |         |         |
|         |         | Key"    |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ### Con |         |         |         |         |         |         |
| vert to |         |         |         |         |         |         |
|  Multis |         |         |         |         |         |         |
| ig {#Te |         |         |         |         |         |         |
| stRepor |         |         |         |         |         |         |
| t-1.2.4 |         |         |         |         |         |         |
| -1-Conv |         |         |         |         |         |         |
| erttoMu |         |         |         |         |         |         |
| ltisig} |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| CV      | Convert | Click   | If      | [PASS]  |         | [YES]   |
| TMTSG-1 | to      | to      | account | {.statu |         | {.statu |
|         | M       | Account | has     | s-macro |         | s-macro |
|         | ultisig | \>      | insuf   | .aui-   |         | .aui-   |
|         |         | M       | ficient | lozenge |         | lozenge |
|         |         | ultisig | xpx (0  | .aui-lo |         | .aui-lo |
|         |         |         | xpx),   | zenge-s |         | zenge-s |
|         |         |         | an      | uccess} |         | uccess} |
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
| CV      | Scheme  | Add and | Value   | [PASS]  |         | [YES]   |
| TMTSG-2 |         | reduce  | does    | {.statu |         | {.statu |
|         |         | approve | not     | s-macro |         | s-macro |
|         |         | trans   | exceed  | .aui-   |         | .aui-   |
|         |         | actions | max     | lozenge |         | lozenge |
|         |         |         | number  | .aui-lo |         | .aui-lo |
|         |         |         | of      | zenge-s |         | zenge-s |
|         |         |         | cosigna | uccess} |         | uccess} |
|         |         |         | tories, |         |         |         |
|         |         |         | and     |         |         |         |
|         |         |         | error   |         |         |         |
|         |         |         | is      |         |         |         |
|         |         |         | shown   |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| CV      |         | Add and | Value   | [PASS]  |         | [YES]   |
| TMTSG-3 |         | reduce  | does    | {.statu |         | {.statu |
|         |         | delete  | not     | s-macro |         | s-macro |
|         |         | users   | exceed  | .aui-   |         | .aui-   |
|         |         |         | max     | lozenge |         | lozenge |
|         |         |         | number  | .aui-lo |         | .aui-lo |
|         |         |         | of      | zenge-s |         | zenge-s |
|         |         |         | cosigna | uccess} |         | uccess} |
|         |         |         | tories, |         |         |         |
|         |         |         | and     |         |         |         |
|         |         |         | error   |         |         |         |
|         |         |         | is      |         |         |         |
|         |         |         | shown   |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| CV      | Add     | Click   | Opens   | [PASS]  |         | [YES]   |
| TMTSG-4 | Cosi    | M       | up      | {.statu |         | {.statu |
|         | gnatory | ultisig | M       | s-macro |         | s-macro |
|         |         | tab     | ultisig | .aui-   |         | .aui-   |
|         |         | under   | S       | lozenge |         | lozenge |
|         |         | a       | ettings | .aui-lo |         | .aui-lo |
|         |         | ccounts |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| CV      |         | Click   | User is | [PASS]  |         | [YES]   |
| TMTSG-5 |         | "Manage | d       | {.statu |         | {.statu |
|         |         | Cosigna | irected | s-macro |         | s-macro |
|         |         | tories" | to      | .aui-   |         | .aui-   |
|         |         | button  | convert | lozenge |         | lozenge |
|         |         | under   | account | .aui-lo |         | .aui-lo |
|         |         | Account | to      | zenge-s |         | zenge-s |
|         |         | \>      | m       | uccess} |         | uccess} |
|         |         | M       | ultisig |         |         |         |
|         |         | ultisig | page    |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| CV      |         | Click   | Opens   | [PASS]  |         | [YES]   |
| TMTSG-6 |         | "Add    | up      | {.statu |         | {.statu |
|         |         | New     | cosi    | s-macro |         | s-macro |
|         |         | Cosig   | gnatory | .aui-   |         | .aui-   |
|         |         | natory" | public  | lozenge |         | lozenge |
|         |         |         | key     | .aui-lo |         | .aui-lo |
|         |         |         | field   | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| CV      |         | Input   | Shows a | [PASS]  |         | [YES]   |
| TMTSG-7 |         | invalid | message | {.statu |         | {.statu |
|         |         | public  | "       | s-macro |         | s-macro |
|         |         | key     | Invalid | .aui-   |         | .aui-   |
|         |         |         | Input"  | lozenge |         | lozenge |
|         |         |         |         | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| CV      |         | Click   | Shows   | [PASS]  |         | [YES]   |
| TMTSG-8 |         | on      | all     | {.statu |         | {.statu |
|         |         | "C      | normal  | s-macro |         | s-macro |
|         |         | ontact" | a       | .aui-   |         | .aui-   |
|         |         | icon    | ccounts | lozenge |         | lozenge |
|         |         |         | and     | .aui-lo |         | .aui-lo |
|         |         |         | c       | zenge-s |         | zenge-s |
|         |         |         | ontacts | uccess} |         | uccess} |
|         |         |         | av      |         |         |         |
|         |         |         | ailable |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| CV      | P       | Leave   | Shows a | [PASS]  |         | [YES]   |
| TMTSG-9 | assword | p       | message | {.statu |         | {.statu |
|         |         | assword | "Wallet | s-macro |         | s-macro |
|         |         | field   | p       | .aui-   |         | .aui-   |
|         |         | empty   | assword | lozenge |         | lozenge |
|         |         |         | is      | .aui-lo |         | .aui-lo |
|         |         |         | re      | zenge-s |         | zenge-s |
|         |         |         | quired" | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| CVT     | Clear   | Click   | User is | [PASS]  |         | [YES]   |
| MTSG-10 |         | "       | d       | {.statu |         | {.statu |
|         |         | Cancel" | irected | s-macro |         | s-macro |
|         |         |         | back to | .aui-   |         | .aui-   |
|         |         |         | m       | lozenge |         | lozenge |
|         |         |         | ultisig | .aui-lo |         | .aui-lo |
|         |         |         | s       | zenge-s |         | zenge-s |
|         |         |         | ettings | uccess} |         | uccess} |
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
| 1.2.4-1 |         |         |         |         |         |         |
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
| ### E   |         |         |         |         |         |         |
| dit Nam |         |         |         |         |         |         |
| espace  |         |         |         |         |         |         |
| {#TestR |         |         |         |         |         |         |
| eport-1 |         |         |         |         |         |         |
| .2.4-1- |         |         |         |         |         |         |
| EditNam |         |         |         |         |         |         |
| espace} |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| EDTN    | Extend  | Click   | D       | [PASS]  |         |         |
| SPACE-1 | D       | "Name   | isplays | {.statu |         |         |
|         | uration | spaces" | Na      | s-macro |         |         |
|         |         | on      | mespace | .aui-   |         |         |
|         |         | Account | Details | lozenge |         |         |
|         |         | Details | page    | .aui-lo |         |         |
|         |         | page    |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| EDTN    |         | Click   | D       | [PASS]  |         |         |
| SPACE-2 |         | "..."   | isplays | {.statu |         |         |
|         |         | under   | option  | s-macro |         |         |
|         |         | "A      | of      | .aui-   |         |         |
|         |         | ctions" | "Extend | lozenge |         |         |
|         |         | column  | Du      | .aui-lo |         |         |
|         |         |         | ration" | zenge-s |         |         |
|         |         |         | and     | uccess} |         |         |
|         |         |         | "View   |         |         |         |
|         |         |         | Me      |         |         |         |
|         |         |         | tadata" |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| EDT     |         | Click   | User is | [PASS]  |         |         |
| NSPACE- |         | "Extend | d       | {.statu |         |         |
| 3       |         | Du      | irected | s-macro |         |         |
|         |         | ration" | to a    | .aui-   |         |         |
|         |         |         | page to | lozenge |         |         |
|         |         |         | extend  | .aui-lo |         |         |
|         |         |         | d       | zenge-s |         |         |
|         |         |         | uration | uccess} |         |         |
|         |         |         | of      |         |         |         |
|         |         |         | Na      |         |         |         |
|         |         |         | mespace |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| EDT     |         | Enter   | User is | [PASS]  |         |         |
| NSPACE- |         | d       | d       | {.statu |         |         |
| 4       |         | uration | irected | s-macro |         |         |
|         |         | of      | to      | .aui-   |         |         |
|         |         | days,\  | tran    | lozenge |         |         |
|         |         | Enter   | saction | .aui-lo |         |         |
|         |         | correct | page    | zenge-s |         |         |
|         |         | p       |         | uccess} |         |         |
|         |         | assword |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| EDT     |         | Enter   | User is | [PASS]  |         |         |
| NSPACE- |         | d       | d       | {.statu |         |         |
| 5       |         | uration | irected | s-macro |         |         |
|         |         | of      | back to | .aui-   |         |         |
|         |         | days,\  | da      | lozenge |         |         |
|         |         | Enter   | shboard | .aui-lo |         |         |
|         |         | correct | page    | zenge-s |         |         |
|         |         | pas     |         | uccess} |         |         |
|         |         | sword,\ |         |         |         |         |
|         |         | Click   |         |         |         |         |
|         |         | "       |         |         |         |         |
|         |         | Cancel" |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| EDT     |         | Enter   | Shows   | [PASS]  |         |         |
| NSPACE- |         | valid   | an      | {.statu |         |         |
| 6       |         | name,\  | error   | s-macro |         |         |
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
| EDT     |         | Enter   | Shows   | [PASS]  |         |         |
| NSPACE- |         | wrong   | an      | {.statu |         |         |
| 7       |         | wallet  | error   | s-macro |         |         |
|         |         | p       | saying  | .aui-   |         |         |
|         |         | assword | wallet  | lozenge |         |         |
|         |         |         | p       | .aui-lo |         |         |
|         |         |         | assword | zenge-s |         |         |
|         |         |         | is      | uccess} |         |         |
|         |         |         | invalid |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ###     |         |         |         |         |         |         |
| Edit As |         |         |         |         |         |         |
| set {#T |         |         |         |         |         |         |
| estRepo |         |         |         |         |         |         |
| rt-1.2. |         |         |         |         |         |         |
| 4-1-Edi |         |         |         |         |         |         |
| tAsset} |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| EDT     | Modify  | Click   | D       | [PASS]  |         |         |
| ASSET-1 | Supply  | "       | isplays | {.statu |         |         |
|         |         | Assets" | Assets  | s-macro |         |         |
|         |         | on      | Details | .aui-   |         |         |
|         |         | Account | page    | lozenge |         |         |
|         |         | Details |         | .aui-lo |         |         |
|         |         | page    |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| EDT     |         | Click   | D       | [PASS]  |         |         |
| ASSET-2 |         | "..."   | isplays | {.statu |         |         |
|         |         | under   | option  | s-macro |         |         |
|         |         | "A      | of      | .aui-   |         |         |
|         |         | ctions" | "Modify | lozenge |         |         |
|         |         | column  | S       | .aui-lo |         |         |
|         |         |         | upply", | zenge-s |         |         |
|         |         |         | "Link   | uccess} |         |         |
|         |         |         | to      |         |         |         |
|         |         |         | Nam     |         |         |         |
|         |         |         | espace" |         |         |         |
|         |         |         | and     |         |         |         |
|         |         |         | "View   |         |         |         |
|         |         |         | Me      |         |         |         |
|         |         |         | tadata" |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ED      |         | Click   | User is | [PASS]  |         |         |
| TASSET- |         | "Modify | d       | {.statu |         |         |
| 3       |         | Supply" | irected | s-macro |         |         |
|         |         |         | to a    | .aui-   |         |         |
|         |         |         | page to | lozenge |         |         |
|         |         |         | modify  | .aui-lo |         |         |
|         |         |         | asset   | zenge-s |         |         |
|         |         |         | supply  | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ED      |         | Click   | "Modify | [PASS]  |         |         |
| TASSET- |         | on      | Asset   | {.statu |         |         |
| 4       |         | "in     | Supply" | s-macro |         |         |
|         |         | crease" | button  | .aui-   |         |         |
|         |         | radio   | is      | lozenge |         |         |
|         |         | button, | disable | .aui-lo |         |         |
|         |         | enter   |         | zenge-s |         |         |
|         |         | "0"     |         | uccess} |         |         |
|         |         | q       |         |         |         |         |
|         |         | uantity |         |         |         |         |
|         |         | of      |         |         |         |         |
|         |         | in      |         |         |         |         |
|         |         | crease. |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ED      |         | Click   | "Modify | [PASS]  |         |         |
| TASSET- |         | on      | Asset   | {.statu |         |         |
| 5       |         | "de     | Supply" | s-macro |         |         |
|         |         | crease" | button  | .aui-   |         |         |
|         |         | radio   | is      | lozenge |         |         |
|         |         | button, | disable | .aui-lo |         |         |
|         |         | enter   |         | zenge-s |         |         |
|         |         | "0"     |         | uccess} |         |         |
|         |         | q       |         |         |         |         |
|         |         | uantity |         |         |         |         |
|         |         | of      |         |         |         |         |
|         |         | de      |         |         |         |         |
|         |         | crease. |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ED      |         | Enter   | User is | [PASS]  |         |         |
| TASSET- |         | valid   | d       | {.statu |         |         |
| 6       |         | qua     | irected | s-macro |         |         |
|         |         | ntity,\ | to      | .aui-   |         |         |
|         |         | Enter   | tran    | lozenge |         |         |
|         |         | correct | saction | .aui-lo |         |         |
|         |         | p       | page    | zenge-s |         |         |
|         |         | assword | and the | uccess} |         |         |
|         |         |         | total   |         |         |         |
|         |         |         | supply  |         |         |         |
|         |         |         | is      |         |         |         |
|         |         |         | updated |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ED      |         | Enter   | User is | [PASS]  |         |         |
| TASSET- |         | valid   | d       | {.statu |         |         |
| 7       |         | qua     | irected | s-macro |         |         |
|         |         | ntity,\ | back to | .aui-   |         |         |
|         |         | Enter   | da      | lozenge |         |         |
|         |         | correct | shboard | .aui-lo |         |         |
|         |         | pas     | page    | zenge-s |         |         |
|         |         | sword,\ |         | uccess} |         |         |
|         |         | Click   |         |         |         |         |
|         |         | "       |         |         |         |         |
|         |         | Cancel" |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ED      |         | Enter   | Shows   | [PASS]  |         |         |
| TASSET- |         | valid   | an      | {.statu |         |         |
| 8       |         | qua     | error   | s-macro |         |         |
|         |         | ntity,\ | saying  | .aui-   |         |         |
|         |         | Leave   | p       | lozenge |         |         |
|         |         | p       | assword | .aui-lo |         |         |
|         |         | assword | is      | zenge-s |         |         |
|         |         | empty   | r       | uccess} |         |         |
|         |         |         | equired |         |         |         |
|         |         |         | and     |         |         |         |
|         |         |         | r       |         |         |         |
|         |         |         | egister |         |         |         |
|         |         |         | button  |         |         |         |
|         |         |         | is      |         |         |         |
|         |         |         | d       |         |         |         |
|         |         |         | isabled |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ED      |         | Enter   | Shows   | [PASS]  |         |         |
| TASSET- |         | wrong   | an      | {.statu |         |         |
| 9       |         | wallet  | error   | s-macro |         |         |
|         |         | p       | saying  | .aui-   |         |         |
|         |         | assword | wallet  | lozenge |         |         |
|         |         |         | p       | .aui-lo |         |         |
|         |         |         | assword | zenge-s |         |         |
|         |         |         | is      | uccess} |         |         |
|         |         |         | invalid |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ED      | Link to | Click   | D       | [PASS]  |         |         |
| TASSET- | Na      | "..."   | isplays | {.statu |         |         |
| 10      | mespace | under   | option  | s-macro |         |         |
|         |         | "A      | of      | .aui-   |         |         |
|         |         | ctions" | "Modify | lozenge |         |         |
|         |         | column  | S       | .aui-lo |         |         |
|         |         |         | upply", | zenge-s |         |         |
|         |         |         | "Link   | uccess} |         |         |
|         |         |         | to      |         |         |         |
|         |         |         | Nam     |         |         |         |
|         |         |         | espace" |         |         |         |
|         |         |         | and     |         |         |         |
|         |         |         | "View   |         |         |         |
|         |         |         | Me      |         |         |         |
|         |         |         | tadata" |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ED      |         | Click   | User is | [PASS]  |         |         |
| TASSET- |         | "Link   | d       | {.statu |         |         |
| 11      |         | to      | irected | s-macro |         |         |
|         |         | Nam     | to a    | .aui-   |         |         |
|         |         | espace" | page to | lozenge |         |         |
|         |         |         | link to | .aui-lo |         |         |
|         |         |         | na      | zenge-s |         |         |
|         |         |         | mespace | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ED      |         | Click   | "Link   | [PASS]  |         |         |
| TASSET- |         | on      | to      | {.statu |         |         |
| 12      |         | "Link"  | Na      | s-macro |         |         |
|         |         | radio   | mespace | .aui-   |         |         |
|         |         | button  | button  | lozenge |         |         |
|         |         | but not | is      | .aui-lo |         |         |
|         |         | se      | disable | zenge-s |         |         |
|         |         | lecting |         | uccess} |         |         |
|         |         | any     |         |         |         |         |
|         |         | Na      |         |         |         |         |
|         |         | mespace |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ED      |         | Click   | "Link   | [PASS]  |         |         |
| TASSET- |         | on      | to      | {.statu |         |         |
| 13      |         | "       | Nam     | s-macro |         |         |
|         |         | Unlink" | espace" | .aui-   |         |         |
|         |         | radio   | button  | lozenge |         |         |
|         |         | button  | is      | .aui-lo |         |         |
|         |         | but not | disable | zenge-s |         |         |
|         |         | se      |         | uccess} |         |         |
|         |         | lecting |         |         |         |         |
|         |         | any     |         |         |         |         |
|         |         | Na      |         |         |         |         |
|         |         | mespace |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ED      |         | Enter   | User is | [PASS]  |         |         |
| TASSET- |         | valid   | d       | {.statu |         |         |
| 14      |         | Na      | irected | s-macro |         |         |
|         |         | mespace | to      | .aui-   |         |         |
|         |         | from    | tran    | lozenge |         |         |
|         |         | d       | saction | .aui-lo |         |         |
|         |         | ropdown | page    | zenge-s |         |         |
|         |         | list,\  |         | uccess} |         |         |
|         |         | Enter   |         |         |         |         |
|         |         | correct |         |         |         |         |
|         |         | p       |         |         |         |         |
|         |         | assword |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ED      |         | Enter   | User is | [PASS]  |         |         |
| TASSET- |         | valid   | d       | {.statu |         |         |
| 15      |         | Na      | irected | s-macro |         |         |
|         |         | mespace | back to | .aui-   |         |         |
|         |         | d       | da      | lozenge |         |         |
|         |         | ropdown | shboard | .aui-lo |         |         |
|         |         | list,\  | page    | zenge-s |         |         |
|         |         | Enter   |         | uccess} |         |         |
|         |         | correct |         |         |         |         |
|         |         | pas     |         |         |         |         |
|         |         | sword,\ |         |         |         |         |
|         |         | Click   |         |         |         |         |
|         |         | "       |         |         |         |         |
|         |         | Cancel" |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ED      |         | Enter   | Shows   | [PASS]  |         |         |
| TASSET- |         | valid   | an      | {.statu |         |         |
| 16      |         | Na      | error   | s-macro |         |         |
|         |         | mespace | saying  | .aui-   |         |         |
|         |         | d       | p       | lozenge |         |         |
|         |         | ropdown | assword | .aui-lo |         |         |
|         |         | list,\  | is      | zenge-s |         |         |
|         |         | Leave   | r       | uccess} |         |         |
|         |         | p       | equired |         |         |         |
|         |         | assword | and     |         |         |         |
|         |         | empty   | r       |         |         |         |
|         |         |         | egister |         |         |         |
|         |         |         | button  |         |         |         |
|         |         |         | is      |         |         |         |
|         |         |         | d       |         |         |         |
|         |         |         | isabled |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ED      |         | Enter   | Shows   | [PASS]  |         |         |
| TASSET- |         | wrong   | an      | {.statu |         |         |
| 17      |         | wallet  | error   | s-macro |         |         |
|         |         | p       | saying  | .aui-   |         |         |
|         |         | assword | wallet  | lozenge |         |         |
|         |         |         | p       | .aui-lo |         |         |
|         |         |         | assword | zenge-s |         |         |
|         |         |         | is      | uccess} |         |         |
|         |         |         | invalid |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
:::

::: table-wrap
+-----------+-----------+-----------+-----------+-----------+---+---+
| ### Out   |           |           |           |           |   |   |
| going Swa |           |           |           |           |   |   |
| p {#TestR |           |           |           |           |   |   |
| eport-1.2 |           |           |           |           |   |   |
| .4-1-Outg |           |           |           |           |   |   |
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
| O         |           | swap when | Swap      | [P        |   |   |
| UTSWAP-17 |           | metx      | tr        | ASS]{.sta |   |   |
|           |           | amount is | ansaction | tus-macro |   |   |
|           |           | higher    | will be   | .au       |   |   |
|           |           | than xpx  | suc       | i-lozenge |   |   |
|           |           | amount in | cessfully | .au       |   |   |
|           |           | the       | created,  | i-lozenge |   |   |
|           |           | account   | not       | -success} |   |   |
|           |           |           | ification |           |   |   |
|           |           |           | prompted  |           |   |   |
|           |           |           | and user  |           |   |   |
|           |           |           | directed  |           |   |   |
|           |           |           | to        |           |   |   |
|           |           |           | s         |           |   |   |
|           |           |           | uccessful |           |   |   |
|           |           |           | swap      |           |   |   |
|           |           |           | details   |           |   |   |
|           |           |           | page      |           |   |   |
+-----------+-----------+-----------+-----------+-----------+---+---+
| O         | Cancel    | Click on  | Swap      | [P        |   |   |
| UTSWAP-18 |           | "Later"   | tr        | ASS]{.sta |   |   |
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
| UTSWAP-19 |           | eye icon  | password  | ASS]{.sta |   |   |
|           |           | button    |           | tus-macro |   |   |
|           |           |           |           | .au       |   |   |
|           |           |           |           | i-lozenge |   |   |
|           |           |           |           | .au       |   |   |
|           |           |           |           | i-lozenge |   |   |
|           |           |           |           | -success} |   |   |
+-----------+-----------+-----------+-----------+-----------+---+---+
| O         | Ce        | Click on  | Ce        | [P        |   |   |
| UTSWAP-20 | rtificate | ce        | rtificate | ASS]{.sta |   |   |
|           |           | rtificate | of the    | tus-macro |   |   |
|           |           |           | swap      | .au       |   |   |
|           |           |           | tr        | i-lozenge |   |   |
|           |           |           | ansaction | .au       |   |   |
|           |           |           | is        | i-lozenge |   |   |
|           |           |           | available | -success} |   |   |
|           |           |           | to be     |           |   |   |
|           |           |           | d         |           |   |   |
|           |           |           | ownloaded |           |   |   |
+-----------+-----------+-----------+-----------+-----------+---+---+
| O         | Done      | Click on  | User      | [P        |   |   |
| UTSWAP-21 |           | Done      | directed  | ASS]{.sta |   |   |
|           |           | after     | back to   | tus-macro |   |   |
|           |           | checking  | swap page | .au       |   |   |
|           |           | on        |           | i-lozenge |   |   |
|           |           | checkbox  |           | .au       |   |   |
|           |           | "I        |           | i-lozenge |   |   |
|           |           | confirm   |           | -success} |   |   |
|           |           | that I    |           |           |   |   |
|           |           | have      |           |           |   |   |
|           |           | d         |           |           |   |   |
|           |           | ownloaded |           |           |   |   |
|           |           | a copy of |           |           |   |   |
|           |           | my        |           |           |   |   |
|           |           | cer       |           |           |   |   |
|           |           | tificate" |           |           |   |   |
+-----------+-----------+-----------+-----------+-----------+---+---+
| O         |           | Click on  | Unable to | [P        |   |   |
| UTSWAP-22 |           | Done      | proceed   | ASS]{.sta |   |   |
|           |           | **        | to swap   | tus-macro |   |   |
|           |           | without** | page      | .au       |   |   |
|           |           | checking  |           | i-lozenge |   |   |
|           |           | on        |           | .au       |   |   |
|           |           | checkbox  |           | i-lozenge |   |   |
|           |           | "I        |           | -success} |   |   |
|           |           | confirm   |           |           |   |   |
|           |           | that I    |           |           |   |   |
|           |           | have      |           |           |   |   |
|           |           | d         |           |           |   |   |
|           |           | ownloaded |           |           |   |   |
|           |           | a copy of |           |           |   |   |
|           |           | my        |           |           |   |   |
|           |           | cer       |           |           |   |   |
|           |           | tificate" |           |           |   |   |
+-----------+-----------+-----------+-----------+-----------+---+---+
:::

::: table-wrap
+-----------+-----------+-----------+-----------+-----------+---+---+
| ### Inc   |           |           |           |           |   |   |
| oming Swa |           |           |           |           |   |   |
| p {#TestR |           |           |           |           |   |   |
| eport-1.2 |           |           |           |           |   |   |
| .4-1-Inco |           |           |           |           |   |   |
| mingSwap} |           |           |           |           |   |   |
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
| INSWAP-17 | Ce        | Click on  | Ce        | [P        |   |   |
|           | rtificate | ce        | rtificate | ASS]{.sta |   |   |
|           |           | rtificate | of the    | tus-macro |   |   |
|           |           |           | swap      | .au       |   |   |
|           |           |           | tr        | i-lozenge |   |   |
|           |           |           | ansaction | .au       |   |   |
|           |           |           | is        | i-lozenge |   |   |
|           |           |           | available | -success} |   |   |
|           |           |           | to be     |           |   |   |
|           |           |           | d         |           |   |   |
|           |           |           | ownloaded |           |   |   |
+-----------+-----------+-----------+-----------+-----------+---+---+
| INSWAP-18 | Done      | Click on  | User      | [P        |   |   |
|           |           | Done      | directed  | ASS]{.sta |   |   |
|           |           | after     | back to   | tus-macro |   |   |
|           |           | checking  | swap page | .au       |   |   |
|           |           | on        |           | i-lozenge |   |   |
|           |           | checkbox  |           | .au       |   |   |
|           |           | "I        |           | i-lozenge |   |   |
|           |           | confirm   |           | -success} |   |   |
|           |           | that I    |           |           |   |   |
|           |           | have      |           |           |   |   |
|           |           | d         |           |           |   |   |
|           |           | ownloaded |           |           |   |   |
|           |           | a copy of |           |           |   |   |
|           |           | my        |           |           |   |   |
|           |           | cer       |           |           |   |   |
|           |           | tificate" |           |           |   |   |
+-----------+-----------+-----------+-----------+-----------+---+---+
| INSWAP-19 |           | Click on  | Unable to | [P        |   |   |
|           |           | Done      | proceed   | ASS]{.sta |   |   |
|           |           | **        | to swap   | tus-macro |   |   |
|           |           | without** | page      | .au       |   |   |
|           |           | checking  |           | i-lozenge |   |   |
|           |           | on        |           | .au       |   |   |
|           |           | checkbox  |           | i-lozenge |   |   |
|           |           | "I        |           | -success} |   |   |
|           |           | confirm   |           |           |   |   |
|           |           | that I    |           |           |   |   |
|           |           | have      |           |           |   |   |
|           |           | d         |           |           |   |   |
|           |           | ownloaded |           |           |   |   |
|           |           | a copy of |           |           |   |   |
|           |           | my        |           |           |   |   |
|           |           | cer       |           |           |   |   |
|           |           | tificate" |           |           |   |   |
+-----------+-----------+-----------+-----------+-----------+---+---+
:::

## Services {#TestReport-1.2.4-1-Services}

### Swap {#TestReport-1.2.4-1-Swap}

#### NIS1 {#TestReport-1.2.4-1-NIS1 style="margin-left: 30.0px;"}

#### ETH {#TestReport-1.2.4-1-ETH style="margin-left: 30.0px;"}

#### BSC {#TestReport-1.2.4-1-BSC style="margin-left: 30.0px;"}

### Wallets {#TestReport-1.2.4-1-Wallets}

#### Change Password {#TestReport-1.2.4-1-ChangePassword style="margin-left: 30.0px;"}

### Voting {#TestReport-1.2.4-1-Voting}

#### Create Poll {#TestReport-1.2.4-1-CreatePoll style="margin-left: 30.0px;"}

#### Vote {#TestReport-1.2.4-1-Vote style="margin-left: 30.0px;"}

#### View Results {#TestReport-1.2.4-1-ViewResults style="margin-left: 30.0px;"}

### Storage {#TestReport-1.2.4-1-Storage}

#### Files {#TestReport-1.2.4-1-Files style="margin-left: 30.0px;"}

#### Upload File {#TestReport-1.2.4-1-UploadFile style="margin-left: 30.0px;"}

#### Send/Share {#TestReport-1.2.4-1-Send/Share style="margin-left: 30.0px;"}

### Sirius Gift {#TestReport-1.2.4-1-SiriusGift}

#### Create {#TestReport-1.2.4-1-Create style="margin-left: 30.0px;"}

#### Redeem {#TestReport-1.2.4-1-Redeem style="margin-left: 30.0px;"}

### Aggregate Transactions {#TestReport-1.2.4-1-AggregateTransactions}

#### Complete {#TestReport-1.2.4-1-Complete style="margin-left: 30.0px;"}

#### Bonded {#TestReport-1.2.4-1-Bonded style="margin-left: 30.0px;"}
:::

::: {.pageSection .group}
::: pageSectionHeader
## Attachments: {#attachments .pageSectionTitle}
:::

::: {.greybox align="left"}
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2537521197/2537521211)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[b6Y7vdCjGYj4Iz0F_WS65i2cmIOlSUT86qa6i_8b-nI5nMCdfPd8pzyZ7F00oJUCaExJm6trTRKlkKGVJ7Sk77IHaRM8J3xiPRDc7QBvZKdGSgTdYDf5PENJN1AGkDy16cx3ElRHYzDKpmmMJA](attachments/2537521197/2537521214)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[-bO8lWnCxvS5X986IxWgckBxaJCAbxhYl3-TF3royi6Q4j9TP6fotHOWiQ-il3_ryQNouMJ4csO5ZSgD_ZjKbkejc_edkj4PbVtm6f83nPyVS5LMbxvR1CSNaPwQrwZqw6pPpu1WRhThCx6m3A](attachments/2537521197/2537521217)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[JuJFRQviEuNr-LFhKKtzgok1mpF5HDikOIL1_xWg6aGr2qkQ8QSbxpffBmBBZjHP0mp8bWeQOwXRWRwlDCdz6gs25qus8boYnGvW4GVGSyi0cdVFcdwMCJyRp_oVci2AbNXYamEotatFLomrkg](attachments/2537521197/2537521220)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[image-20220321-013652.png](attachments/2537521197/2537521223.png)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[image-20220321-033506.png](attachments/2537521197/2537521226.png)
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
