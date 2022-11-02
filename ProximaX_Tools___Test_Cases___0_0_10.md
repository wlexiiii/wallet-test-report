::: {#page}
::: {#main .aui-page-panel}
::: {#main-header}
::: {#breadcrumb-section}
1.  [ProximaX Tools](index.html)
2.  [Test Reports](Test-Reports_2443871313.html)
:::

# [ ProximaX Tools : Test Cases - 0.0.10 ]{#title-text} {#title-heading .pagetitle}
:::

::: {#content .view}
::: page-metadata
Created by [ Shin Neng]{.author}, last modified by [ Shi Hui
Khoo]{.editor} on Jan 19, 2022
:::

::: {#main-content .wiki-content .group}
Date: 30/11/2021 - 2/12/2021\
Version: 0.0.10\
Test Environment: Chrome (Version 96.0.4664.45), Windows 10, Core
i7-1165G7 CPU, 16GB RAM\
Staging Link: [ProximaX Web Wallet
(proximax-foundry.github.io)](https://proximax-foundry.github.io/web-wallet-vuejs/#/){.external-link
rel="nofollow"}\
Browser: Google Chrome (Version 96.0.4664.45)\
Testnet: Testnet 1\

::: {.toc-macro .rbtoc1667369960994}
-   [Main Page](#TestCases-0.0.10-MainPage)
    -   [Sign In](#TestCases-0.0.10-SignIn)
    -   [Sign In With SiriusID](#TestCases-0.0.10-SignInWithSiriusID)
    -   [Create New Wallet](#TestCases-0.0.10-CreateNewWallet)
    -   [Create New Wallet From Private
        Key](#TestCases-0.0.10-CreateNewWalletFromPrivateKey)
    -   [Import wallet from .wlt file (Create Wallet from a Wallet
        Backup)](#TestCases-0.0.10-Importwalletfrom.wltfile(CreateWalletfromaWalletBackup))
-   [Dashboard](#TestCases-0.0.10-Dashboard)
-   [Side Menu Bar (Home Page)](#TestCases-0.0.10-SideMenuBar(HomePage))
-   [Transfer (New Design)](#TestCases-0.0.10-Transfer(NewDesign))
-   [Transfer (Not applicable for
    now)](#TestCases-0.0.10-Transfer(Notapplicablefornow))
-   [Accounts](#TestCases-0.0.10-Accounts)
    -   [Select Creation Type](#TestCases-0.0.10-SelectCreationType)
        -   [Create a New Account in the same
            Wallet](#TestCases-0.0.10-CreateaNewAccountinthesameWallet)
        -   [Create a New Account from Private Key in the same
            Wallet](#TestCases-0.0.10-CreateaNewAccountfromPrivateKeyinthesameWallet)
    -   [Edit an existing
        Account](#TestCases-0.0.10-EditanexistingAccount)
        -   [Details](#TestCases-0.0.10-Details)
    -   [Convert to Multisig](#TestCases-0.0.10-ConverttoMultisig)
    -   [Edit Multisig](#TestCases-0.0.10-EditMultisig)
-   [Services](#TestCases-0.0.10-Services)
    -   [Namespaces](#TestCases-0.0.10-Namespaces)
        -   [Register](#TestCases-0.0.10-Register)
        -   [Extend Duration](#TestCases-0.0.10-ExtendDuration)
    -   [Assets](#TestCases-0.0.10-Assets)
        -   [Create](#TestCases-0.0.10-Create)
        -   [Modify Supply](#TestCases-0.0.10-ModifySupply)
        -   [Link to Namespaces](#TestCases-0.0.10-LinktoNamespaces)
    -   [Swap](#TestCases-0.0.10-Swap)
        -   [NIS1](#TestCases-0.0.10-NIS1)
        -   [ETH](#TestCases-0.0.10-ETH)
        -   [BSC](#TestCases-0.0.10-BSC)
    -   [Address Book](#TestCases-0.0.10-AddressBook)
        -   [List](#TestCases-0.0.10-List)
        -   [Add Contacts](#TestCases-0.0.10-AddContacts)
    -   [Wallets](#TestCases-0.0.10-Wallets)
        -   [Change Password](#TestCases-0.0.10-ChangePassword)
        -   [Export](#TestCases-0.0.10-Export)
        -   [Delete](#TestCases-0.0.10-Delete)
    -   [Voting](#TestCases-0.0.10-Voting)
        -   [Create Poll](#TestCases-0.0.10-CreatePoll)
        -   [Vote](#TestCases-0.0.10-Vote)
        -   [View Results](#TestCases-0.0.10-ViewResults)
    -   [Storage](#TestCases-0.0.10-Storage)
        -   [Files](#TestCases-0.0.10-Files)
        -   [Upload File](#TestCases-0.0.10-UploadFile)
        -   [Send/Share](#TestCases-0.0.10-Send/Share)
    -   [Sirius Gift](#TestCases-0.0.10-SiriusGift)
        -   [Create](#TestCases-0.0.10-Create.1)
        -   [Redeem](#TestCases-0.0.10-Redeem)
    -   [Aggregate
        Transactions](#TestCases-0.0.10-AggregateTransactions)
        -   [Complete](#TestCases-0.0.10-Complete)
        -   [Bonded](#TestCases-0.0.10-Bonded)
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
| ## Mai  |         |         |         |         |         |         |
| n Page  |         |         |         |         |         |         |
| {#TestC |         |         |         |         |         |         |
| ases-0. |         |         |         |         |         |         |
| 0.10-Ma |         |         |         |         |         |         |
| inPage} |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| **Test  | **Test  | **Test  | **E     | **S     | **R     | **Auto  |
| Case    | Scen    | steps** | xpected | tatus** | emark** | mated** |
| ID**    | arios** |         | r       |         |         |         |
|         |         |         | esult** |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| Main-1  | Sign in | Select  | Unable  | [FAIL]  | Error   | \-      |
|         |         | wallet  | to sign | {.statu | not     |         |
|         |         | and     | in,     | s-macro | shown   |         |
|         |         | click   | "Sign   | .aui-   |         |         |
|         |         | on      | In"     | lozenge |         |         |
|         |         | "Sign   | button  | .aui-   |         |         |
|         |         | in"     | is      | lozenge |         |         |
|         |         | button  | d       | -error} |         |         |
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
| Main-4  | Sign in | Click   | Show    | [NOT    |         | \-      |
|         | with    | on      | the     | READY]  |         |         |
|         | S       | "Sign   | form    | {.statu |         |         |
|         | iriusID | in with | "Sign   | s-macro |         |         |
|         |         | Si      | in your | .aui-l  |         |         |
|         |         | riusID" | wallet  | ozenge} |         |         |
|         |         | button  | by      |         |         |         |
|         |         |         | s       |         |         |         |
|         |         |         | canning |         |         |         |
|         |         |         | this QR |         |         |         |
|         |         |         | Code    |         |         |         |
|         |         |         | using   |         |         |         |
|         |         |         | your    |         |         |         |
|         |         |         | S       |         |         |         |
|         |         |         | iriusID |         |         |         |
|         |         |         | app"    |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| Main-5  | Create  | Click   | Go to   | [PASS]  |         | [YES]   |
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
| ###     |         |         |         |         |         |         |
|  Sign I |         |         |         |         |         |         |
| n {#Tes |         |         |         |         |         |         |
| tCases- |         |         |         |         |         |         |
| 0.0.10- |         |         |         |         |         |         |
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
| S       |         | Place   | Show    | [FAIL]  | Does    | \-      |
| IGNIN-2 |         | less    | message | {.statu | not     |         |
|         |         | than    | of      | s-macro | show    |         |
|         |         | r       | minimum | .aui-   | error   |         |
|         |         | equired | number  | lozenge | m       |         |
|         |         | values  | of      | .aui-   | essage, |         |
|         |         |         | cha     | lozenge | sign in |         |
|         |         |         | racters | -error} | button  |         |
|         |         |         | to      |         | is      |         |
|         |         |         | enter   |         | d       |         |
|         |         |         |         |         | isabled |         |
|         |         |         |         |         | instead |         |
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
| S       |         | Click   | Clear   | [NOT    |         | \-      |
| IGNIN-5 |         | on      | the     | READY]  |         |         |
|         |         | "Clear" | form    | {.statu |         |         |
|         |         | button  |         | s-macro |         |         |
|         |         |         |         | .aui-l  |         |         |
|         |         |         |         | ozenge} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| S       | General | UI      | N/A     | \-      |         | \-      |
| IGNIN-6 | form    | verif   |         |         |         |         |
|         |         | ication |         |         |         |         |
|         |         | (       |         |         |         |         |
|         |         | syntax) |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| S       | Sign    | Click   | Go back | [PASS]  |         | [YES]   |
| IGNIN-7 | Out     | on      | to Sign | {.statu |         | {.statu |
|         |         | "Sign   | In page | s-macro |         | s-macro |
|         |         | Out"    |         | .aui-   |         | .aui-   |
|         |         | button  |         | lozenge |         | lozenge |
|         |         |         |         | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| #       |         |         |         |         | [NOT    |         |
| ## Sign |         |         |         |         | READY]  |         |
|  In Wit |         |         |         |         | {.statu |         |
| h Siriu |         |         |         |         | s-macro |         |
| sID {#T |         |         |         |         | .aui-l  |         |
| estCase |         |         |         |         | ozenge} |         |
| s-0.0.1 |         |         |         |         |         |         |
| 0-SignI |         |         |         |         |         |         |
| nWithSi |         |         |         |         |         |         |
| riusID} |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
|         |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| #       |         |         |         |         |         |         |
| ## Crea |         |         |         |         |         |         |
| te New  |         |         |         |         |         |         |
| Wallet  |         |         |         |         |         |         |
| {#TestC |         |         |         |         |         |         |
| ases-0. |         |         |         |         |         |         |
| 0.10-Cr |         |         |         |         |         |         |
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
| N       |         | Set     | N/A     | \-      |         | \-      |
| EWWLT-3 |         | special |         |         |         |         |
|         |         | cha     |         |         |         |         |
|         |         | racters |         |         |         |         |
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
|         |         |         | 8, max  | lozenge |         | lozenge |
|         |         |         | length  | .aui-lo |         | .aui-lo |
|         |         |         | 30"     | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| N       |         | Set     | N/A     | \-      |         | \-      |
| EWWLT-6 |         | special |         |         |         |         |
|         |         | cha     |         |         |         |         |
|         |         | racters |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| N       |         | Place   | Show    | [PASS]  |         | [YES]   |
| EWWLT-7 |         | less or | message | {.statu |         | {.statu |
|         |         | more    | of      | s-macro |         | s-macro |
|         |         | than    | minimum | .aui-   |         | .aui-   |
|         |         | r       | and     | lozenge |         | lozenge |
|         |         | equired | maximum | .aui-lo |         | .aui-lo |
|         |         | values  | number  | zenge-s |         | zenge-s |
|         |         |         | of      | uccess} |         | uccess} |
|         |         |         | cha     |         |         |         |
|         |         |         | racters |         |         |         |
|         |         |         | to      |         |         |         |
|         |         |         | enter\  |         |         |         |
|         |         |         | "min    |         |         |         |
|         |         |         | length  |         |         |         |
|         |         |         | 8, max  |         |         |         |
|         |         |         | length  |         |         |         |
|         |         |         | 30"     |         |         |         |
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
| NE      |         | Set     | N/A     | \-      |         | \-      |
| WWLT-10 |         | special |         |         |         |         |
|         |         | cha     |         |         |         |         |
|         |         | racters |         |         |         |         |
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
| NE      | Clear   | Click   | Clean   | [NOT    |         | \-      |
| WWLT-14 |         | on      | the     | READY]  |         |         |
|         |         | "Clear" | form    | {.statu |         |         |
|         |         | button  |         | s-macro |         |         |
|         |         |         |         | .aui-l  |         |         |
|         |         |         |         | ozenge} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      | Create  | Click   | Send a  | [PASS]  |         | [YES]   |
| WWLT-15 |         | on      | confi   | {.statu |         | {.statu |
|         |         | "Create | rmation | s-macro |         | s-macro |
|         |         | Wallet" | message | .aui-   |         | .aui-   |
|         |         | button  | and     | lozenge |         | lozenge |
|         |         |         | create  | .aui-lo |         | .aui-lo |
|         |         |         | the     | zenge-s |         | zenge-s |
|         |         |         | wallet  | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| ###     |         |         |         |         |         |         |
| Create  |         |         |         |         |         |         |
| New Wal |         |         |         |         |         |         |
| let Fro |         |         |         |         |         |         |
| m Priva |         |         |         |         |         |         |
| te Key  |         |         |         |         |         |         |
| {#TestC |         |         |         |         |         |         |
| ases-0. |         |         |         |         |         |         |
| 0.10-Cr |         |         |         |         |         |         |
| eateNew |         |         |         |         |         |         |
| WalletF |         |         |         |         |         |         |
| romPriv |         |         |         |         |         |         |
| ateKey} |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      | Create  | Click   | Go to   | [PASS]  |         | [YES]   |
| WWLT-16 | Wallet\ | on      | screen  | {.statu |         | {.statu |
|         | (From a | Create  | "Create | s-macro |         | s-macro |
|         | Private | Wallet  | Wallet  | .aui-   |         | .aui-   |
|         | Key)    | "From a | from a  | lozenge |         | lozenge |
|         |         | Private | Private | .aui-lo |         | .aui-lo |
|         |         | Key"    | Key"    | zenge-s |         | zenge-s |
|         |         | button  |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| NE      | Private | Leave   | Show an | [PASS]  |         | [YES]   |
| WWLT-17 | key     | the     | error   | {.statu |         | {.statu |
|         |         | field   | message | s-macro |         | s-macro |
|         |         | empty   | "       | .aui-   |         | .aui-   |
|         |         |         | Invalid | lozenge |         | lozenge |
|         |         |         | private | .aui-lo |         | .aui-lo |
|         |         |         | key"    | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Set an  | Show an | [PASS]  |         | [YES]   |
| WWLT-18 |         | invalid | error   | {.statu |         | {.statu |
|         |         | value   | message | s-macro |         | s-macro |
|         |         |         | "       | .aui-   |         | .aui-   |
|         |         |         | Invalid | lozenge |         | lozenge |
|         |         |         | private | .aui-lo |         | .aui-lo |
|         |         |         | key"    | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| NE      | Swap    | Click   | Check   | [NOT    |         | \-      |
| WWLT-19 |         | on      | the     | READY]  |         |         |
|         |         | c       | option  | {.statu |         |         |
|         |         | heckbox |         | s-macro |         |         |
|         |         |         |         | .aui-l  |         |         |
|         |         |         |         | ozenge} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      | Wallet  | Leave   | Show a  | [PASS]  |         | [YES]   |
| WWLT-20 | name    | the     | message | {.statu |         | {.statu |
|         |         | field   | "Enter  | s-macro |         | s-macro |
|         |         | empty   | Wallet  | .aui-   |         | .aui-   |
|         |         |         | Name"   | lozenge |         | lozenge |
|         |         |         |         | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Set     | N/A     | \-      |         | \-      |
| WWLT-21 |         | special |         |         |         |         |
|         |         | cha     |         |         |         |         |
|         |         | racters |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      | Pa      | Leave   | Show a  | [PASS]  |         | [YES]   |
| WWLT-22 | ssword  | the     | message | {.statu |         | {.statu |
|         |         | field   | "min    | s-macro |         | s-macro |
|         |         | empty   | length  | .aui-   |         | .aui-   |
|         |         |         | 8, max  | lozenge |         | lozenge |
|         |         |         | length  | .aui-lo |         | .aui-lo |
|         |         |         | 30"\    | zenge-s |         | zenge-s |
|         |         |         | "Please | uccess} |         | uccess} |
|         |         |         | enter a |         |         |         |
|         |         |         | pa      |         |         |         |
|         |         |         | ssword" |         |         |         |
|         |         |         | i       |         |         |         |
|         |         |         | nstead? |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Set an  | Show a  | [PASS]  |         | [YES]   |
| WWLT-23 |         | invalid | message | {.statu |         | {.statu |
|         |         | p       | "min    | s-macro |         | s-macro |
|         |         | assword | length  | .aui-   |         | .aui-   |
|         |         |         | 8, max  | lozenge |         | lozenge |
|         |         |         | length  | .aui-lo |         | .aui-lo |
|         |         |         | 30"     | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Set     | N/A     | \-      |         | \-      |
| WWLT-24 |         | special |         |         |         |         |
|         |         | cha     |         |         |         |         |
|         |         | racters |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Place   | Show    | [PASS]  |         | [YES]   |
| WWLT-25 |         | less or | message | {.statu |         | {.statu |
|         |         | more    | of      | s-macro |         | s-macro |
|         |         | than    | minimum | .aui-   |         | .aui-   |
|         |         | r       | and     | lozenge |         | lozenge |
|         |         | equired | maximum | .aui-lo |         | .aui-lo |
|         |         | values  | number  | zenge-s |         | zenge-s |
|         |         |         | of      | uccess} |         | uccess} |
|         |         |         | cha     |         |         |         |
|         |         |         | racters |         |         |         |
|         |         |         | to      |         |         |         |
|         |         |         | enter\  |         |         |         |
|         |         |         | "min    |         |         |         |
|         |         |         | length  |         |         |         |
|         |         |         | 8, max  |         |         |         |
|         |         |         | length  |         |         |         |
|         |         |         | 30"     |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      | Confirm | Leave   | Show a  | [PASS]  |         | [YES]   |
| WWLT-26 | p       | the     | message | {.statu |         | {.statu |
|         | assword | field   | "P      | s-macro |         | s-macro |
|         |         | empty   | assword | .aui-   |         | .aui-   |
|         |         |         | doesn't | lozenge |         | lozenge |
|         |         |         | match"  | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Enter a | Show a  | [PASS]  |         | [YES]   |
| WWLT-27 |         | di      | message | {.statu |         | {.statu |
|         |         | fferent | "P      | s-macro |         | s-macro |
|         |         | p       | assword | .aui-   |         | .aui-   |
|         |         | assword | doesn't | lozenge |         | lozenge |
|         |         |         | match"  | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Set     | N/A     | \-      |         | \-      |
| WWLT-28 |         | special |         |         |         |         |
|         |         | cha     |         |         |         |         |
|         |         | racters |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Place   | Show a  | [PASS]  |         | [YES]   |
| WWLT-29 |         | less or | message | {.statu |         | {.statu |
|         |         | more    | "P      | s-macro |         | s-macro |
|         |         | than    | assword | .aui-   |         | .aui-   |
|         |         | r       | doesn't | lozenge |         | lozenge |
|         |         | equired | match"\ | .aui-lo |         | .aui-lo |
|         |         | values  |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| NE      | Eye     | Click   | Show /  | [PASS]  |         | [YES]   |
| WWLT-30 | icons   | on      | hide    | {.statu |         | {.statu |
|         |         | "       | the     | s-macro |         | s-macro |
|         |         | Private | private | .aui-   |         | .aui-   |
|         |         | key"    | key     | lozenge |         | lozenge |
|         |         | eye     |         | .aui-lo |         | .aui-lo |
|         |         | icon    |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Click   | Show /  | [PASS]  |         | [YES]   |
| WWLT-31 |         | on      | hide    | {.statu |         | {.statu |
|         |         | "Pa     | the     | s-macro |         | s-macro |
|         |         | ssword" | p       | .aui-   |         | .aui-   |
|         |         | eye     | assword | lozenge |         | lozenge |
|         |         | icon    |         | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Click   | Show /  | [PASS]  |         | [YES]   |
| WWLT-32 |         | on      | hide    | {.statu |         | {.statu |
|         |         | "       | the     | s-macro |         | s-macro |
|         |         | Confirm | p       | .aui-   |         | .aui-   |
|         |         | pa      | assword | lozenge |         | lozenge |
|         |         | ssword" |         | .aui-lo |         | .aui-lo |
|         |         | eye     |         | zenge-s |         | zenge-s |
|         |         | icon    |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| NE      | N/A     | Click   | Clean   | [NOT    |         | \-      |
| WWLT-33 |         | on      | the     | READY]  |         |         |
|         |         | "Clear" | form    | {.statu |         |         |
|         |         | button  |         | s-macro |         |         |
|         |         |         |         | .aui-l  |         |         |
|         |         |         |         | ozenge} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Click   | Send a  | [PASS]  |         | [YES]   |
| WWLT-34 |         | on      | confi   | {.statu |         | {.statu |
|         |         | "       | rmation | s-macro |         | s-macro |
|         |         | Create" | message | .aui-   |         | .aui-   |
|         |         | button  | and     | lozenge |         | lozenge |
|         |         |         | create  | .aui-lo |         | .aui-lo |
|         |         |         | the     | zenge-s |         | zenge-s |
|         |         |         | wallet  | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| NE      | General | UI      | N/A     | \-      |         | \-      |
| WWLT-35 | form    | verif   |         |         |         |         |
|         |         | ication |         |         |         |         |
|         |         | (       |         |         |         |         |
|         |         | syntax) |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ### I   |         |         |         |         |         |         |
| mport w |         |         |         |         |         |         |
| allet f |         |         |         |         |         |         |
| rom .wl |         |         |         |         |         |         |
| t file  |         |         |         |         |         |         |
| (Create |         |         |         |         |         |         |
|  Wallet |         |         |         |         |         |         |
|  from a |         |         |         |         |         |         |
|  Wallet |         |         |         |         |         |         |
|  Backup |         |         |         |         |         |         |
| ) {#Tes |         |         |         |         |         |         |
| tCases- |         |         |         |         |         |         |
| 0.0.10- |         |         |         |         |         |         |
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
| WWLT-37 | (From a | on      | screen  | {.statu |         | {.statu |
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
| WWLT-38 |         | have a  | to Sign | {.statu |         | {.statu |
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
| ## Dash |         |         |         |         |         |         |
| board { |         |         |         |         |         |         |
| #TestCa |         |         |         |         |         |         |
| ses-0.0 |         |         |         |         |         |         |
| .10-Das |         |         |         |         |         |         |
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
| DASH-6  | Beg     | Click   | A list  | [NOT    |         | \-      |
|         | inner's | on      | of      | READY]  |         |         |
|         | guide   | q       | b       | {.statu |         |         |
|         |         | uestion | eginner | s-macro |         |         |
|         |         | mark    | guides  | .aui-l  |         |         |
|         |         | button  | av      | ozenge} |         |         |
|         |         |         | ailable |         |         |         |
|         |         |         | for     |         |         |         |
|         |         |         | user    |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-7  | Notif   |         |         | [NOT    |         | \-      |
|         | ication |         |         | READY]  |         |         |
|         |         |         |         | {.statu |         |         |
|         |         |         |         | s-macro |         |         |
|         |         |         |         | .aui-l  |         |         |
|         |         |         |         | ozenge} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-8  | S       |         |         | [NOT    |         | \-      |
|         | ettings |         |         | READY]  |         |         |
|         |         |         |         | {.statu |         |         |
|         |         |         |         | s-macro |         |         |
|         |         |         |         | .aui-l  |         |         |
|         |         |         |         | ozenge} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| DASH-9  | O       | Click   | An      | [PASS]  |         | [YES]   |
|         | verview | on      | o       | {.statu |         | {.statu |
|         |         | "Ov     | verview | s-macro |         | s-macro |
|         |         | erview" | of      | .aui-   |         | .aui-   |
|         |         | tab     | user's  | lozenge |         | lozenge |
|         |         |         | assets, | .aui-lo |         | .aui-lo |
|         |         |         | nam     | zenge-s |         | zenge-s |
|         |         |         | espaces | uccess} |         | uccess} |
|         |         |         | and     |         |         |         |
|         |         |         | recent  |         |         |         |
|         |         |         | trans   |         |         |         |
|         |         |         | actions |         |         |         |
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
| DASH-14 |         | Click   | User is | [PASS]  |         | [YES]   |
|         |         | on      | d       | {.statu |         | {.statu |
|         |         | "T      | irected | s-macro |         | s-macro |
|         |         | ransfer | to      | .aui-   |         | .aui-   |
|         |         | XPX\'   | create  | lozenge |         | lozenge |
|         |         | button  | t       | .aui-lo |         | .aui-lo |
|         |         |         | ransfer | zenge-s |         | zenge-s |
|         |         |         | page    | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
:::

::: table-wrap
+---------+---------+---------+---------+---------+---------+---------+
| ## Side |         |         |         |         |         |         |
|  Menu B |         |         |         |         |         |         |
| ar (Hom |         |         |         |         |         |         |
| e Page) |         |         |         |         |         |         |
|  {#Test |         |         |         |         |         |         |
| Cases-0 |         |         |         |         |         |         |
| .0.10-S |         |         |         |         |         |         |
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
|         |         |         |         |         |         | (under  |
|         |         |         |         |         |         | create  |
|         |         |         |         |         |         | account |
|         |         |         |         |         |         | test)   |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-2  | Create  | Click   | User is | [PASS]  |         | [YES]   |
|         | New     | on      | d       | {.statu |         | {.statu |
|         | Account | "       | irected | s-macro |         | s-macro |
|         |         | +Create | to      | .aui-   |         | .aui-   |
|         |         | New     | "Create | lozenge |         | lozenge |
|         |         | A       | New     | .aui-lo |         | .aui-lo |
|         |         | ccount" | A       | zenge-s |         | zenge-s |
|         |         | under   | ccount" | uccess} |         | uccess} |
|         |         | "Ac     | Page    |         |         | (under  |
|         |         | counts" |         |         |         | create  |
|         |         |         |         |         |         | account |
|         |         |         |         |         |         | test)   |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-3  | Na      | Click   | User is | [PASS]  |         | [YES]   |
|         | mespace | on      | d       | {.statu |         | {.statu |
|         |         | "Nam    | irected | s-macro |         | s-macro |
|         |         | espace" | to a    | .aui-   |         | .aui-   |
|         |         | under   | page to | lozenge |         | lozenge |
|         |         | "       | create  | .aui-lo |         | .aui-lo |
|         |         | Create" | na      | zenge-s |         | zenge-s |
|         |         |         | mespace | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-4  |         | Leave   | Show an | [NOT    |         | \-      |
|         |         | name    | error   | READY]  |         |         |
|         |         | empty   | message | {.statu |         |         |
|         |         |         | saying  | s-macro |         |         |
|         |         |         | it's a  | .aui-l  |         |         |
|         |         |         | r       | ozenge} |         |         |
|         |         |         | equired |         |         |         |
|         |         |         | field   |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-5  |         | Enter   | Shows   | [PASS]  |         | [YES]   |
|         |         | invalid | an      | {.statu |         | {.statu |
|         |         | name    | error   | s-macro |         | s-macro |
|         |         | (one    | message | .aui-   |         | .aui-   |
|         |         | char)   | to      | lozenge |         | lozenge |
|         |         |         | enter   | .aui-lo |         | .aui-lo |
|         |         |         | valid   | zenge-s |         | zenge-s |
|         |         |         | name    | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-6  |         | Enter   | Na      | [PASS]  |         | [YES]   |
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
| MENU-7  |         | Enter   | User is | [NOT    |         | \-      |
|         |         | valid   | d       | READY]  |         |         |
|         |         | name,\  | irected | {.statu |         |         |
|         |         | Enter   | back to | s-macro |         |         |
|         |         | d       | na      | .aui-l  |         |         |
|         |         | uration | mespace | ozenge} |         |         |
|         |         | of      | page    |         |         |         |
|         |         | days,\  |         |         |         |         |
|         |         | Enter   |         |         |         |         |
|         |         | correct |         |         |         |         |
|         |         | pas     |         |         |         |         |
|         |         | sword,\ |         |         |         |         |
|         |         | Click   |         |         |         |         |
|         |         | "       |         |         |         |         |
|         |         | Cancel" |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-8  |         | Enter   | Shows   | [PASS]  |         | [YES]   |
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
| MENU-9  |         | Enter   | Shows   | [NOT    |         | \-      |
|         |         | wrong   | an      | READY]  |         |         |
|         |         | wallet  | error   | {.statu |         |         |
|         |         | p       | saying  | s-macro |         |         |
|         |         | assword | wallet  | .aui-l  |         |         |
|         |         |         | p       | ozenge} |         |         |
|         |         |         | assword |         |         |         |
|         |         |         | is      |         |         |         |
|         |         |         | in      |         |         |         |
|         |         |         | correct |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-10 | Asset   | Click   | User is | [PASS]  |         | [YES]   |
|         |         | on      | d       | {.statu |         | {.statu |
|         |         | "Asset" | irected | s-macro |         | s-macro |
|         |         | under   | to      | .aui-   |         | .aui-   |
|         |         | "       | "       | lozenge |         | lozenge |
|         |         | Create" | Assets" | .aui-lo |         | .aui-lo |
|         |         |         | page    | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-11 |         | Click   | User is | [PASS]  |         | [YES]   |
|         |         | on      | d       | {.statu |         | {.statu |
|         |         | "       | irected | s-macro |         | s-macro |
|         |         | +Create | to      | .aui-   |         | .aui-   |
|         |         | New     | "Create | lozenge |         | lozenge |
|         |         | Asset"  | Asset"  | .aui-lo |         | .aui-lo |
|         |         |         | page    | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-12 |         | Leave   | Show an | [PASS]  |         | [YES]   |
|         |         | supply, | error   | {.statu |         | {.statu |
|         |         | divis   | to      | s-macro |         | s-macro |
|         |         | ibility | enter   | .aui-   |         | .aui-   |
|         |         | and     | wallet  | lozenge |         | lozenge |
|         |         | wallet  | p       | .aui-lo |         | .aui-lo |
|         |         | p       | assword | zenge-s |         | zenge-s |
|         |         | assword |         | uccess} |         | uccess} |
|         |         | empty   |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-13 |         | Enter   | Asset   | [PASS]  |         | [YES]   |
|         |         | amount  | is      | {.statu |         | {.statu |
|         |         | of      | created | s-macro |         | s-macro |
|         |         | s       | with    | .aui-   |         | .aui-   |
|         |         | upply,\ | its     | lozenge |         | lozenge |
|         |         | Enter   | res     | .aui-lo |         | .aui-lo |
|         |         | divisib | pective | zenge-s |         | zenge-s |
|         |         | ility,\ | id and  | uccess} |         | uccess} |
|         |         | Enter   | details |         |         |         |
|         |         | wallet  |         |         |         |         |
|         |         | p       |         |         |         |         |
|         |         | assword |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-14 | Other   |         |         | [NOT    |         | \-      |
|         | s       |         |         | READY]  |         |         |
|         | ervices |         |         | {.statu |         |         |
|         |         |         |         | s-macro |         |         |
|         |         |         |         | .aui-l  |         |         |
|         |         |         |         | ozenge} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-15 | Wallets | Click   | D       | [PASS]  |         | [YES]   |
|         |         | on      | isplays | {.statu |         | {.statu |
|         |         | "W      | a list  | s-macro |         | s-macro |
|         |         | allets" | of      | .aui-   |         | .aui-   |
|         |         | under   | wallets | lozenge |         | lozenge |
|         |         | "Na     | av      | .aui-lo |         | .aui-lo |
|         |         | vigate" | ailable | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-16 |         | Click   | D       | [PASS]  |         | [YES]   |
|         |         | on the  | isplays | {.statu |         | {.statu |
|         |         | X of    | the     | s-macro |         | s-macro |
|         |         | the     | wallets | .aui-   |         | .aui-   |
|         |         | wallet  | detail  | lozenge |         | lozenge |
|         |         | to      | and     | .aui-lo |         | .aui-lo |
|         |         | delete  | asks    | zenge-s |         | zenge-s |
|         |         | it      | for     | uccess} |         | uccess} |
|         |         |         | delete  |         |         |         |
|         |         |         | confi   |         |         |         |
|         |         |         | rmation |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-17 |         | Click   | Wallet  | [PASS]  |         | [YES]   |
|         |         | on      | succe   | {.statu |         | {.statu |
|         |         | delete  | ssfully | s-macro |         | s-macro |
|         |         | now     | removed | .aui-   |         | .aui-   |
|         |         | button  | and a   | lozenge |         | lozenge |
|         |         |         | notif   | .aui-lo |         | .aui-lo |
|         |         |         | ication | zenge-s |         | zenge-s |
|         |         |         | is      | uccess} |         | uccess} |
|         |         |         | shown   |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-18 | A       | Click   | D       | [PASS]  |         | \-      |
|         | ccounts | on      | isplays | {.statu |         |         |
|         |         | "Ac     | an      | s-macro |         |         |
|         |         | counts" | o       | .aui-   |         |         |
|         |         | under   | verview | lozenge |         |         |
|         |         | "Na     | of the  | .aui-lo |         |         |
|         |         | vigate" | user's  | zenge-s |         |         |
|         |         |         | a       | uccess} |         |         |
|         |         |         | ccounts |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-19 |         | Click   | D       | [NOT    |         | \-      |
|         |         | on "My  | isplays | READY]  |         |         |
|         |         | Ac      | user's  | {.statu |         |         |
|         |         | counts" | a       | s-macro |         |         |
|         |         | tab     | ccounts | .aui-l  |         |         |
|         |         |         |         | ozenge} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-20 |         | Click   | D       | [NOT    |         | \-      |
|         |         | on      | isplays | READY]  |         |         |
|         |         | "M      | user's  | {.statu |         |         |
|         |         | ultisig | m       | s-macro |         |         |
|         |         | Ac      | ultisig | .aui-l  |         |         |
|         |         | counts" | a       | ozenge} |         |         |
|         |         | tab     | ccounts |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-21 |         | Click   | D       | [NOT    |         | \-      |
|         |         | on      | isplays | READY]  |         |         |
|         |         | "Other  | user's  | {.statu |         |         |
|         |         | Ac      | other   | s-macro |         |         |
|         |         | counts" | a       | .aui-l  |         |         |
|         |         | tab     | ccounts | ozenge} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-22 | Address | Click   | D       | [PASS]  |         | [YES]   |
|         | Book    | on      | isplays | {.statu |         | {.statu |
|         |         | "       | user's  | s-macro |         | s-macro |
|         |         | Address | address | .aui-   |         | .aui-   |
|         |         | Book"   | book    | lozenge |         | lozenge |
|         |         | under   | list    | .aui-lo |         | .aui-lo |
|         |         | "Na     |         | zenge-s |         | zenge-s |
|         |         | vigate" |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-23 |         | Click   | User    | [PASS]  |         | [YES]   |
|         |         | on      | d       | {.statu |         | {.statu |
|         |         | "+Add   | irected | s-macro |         | s-macro |
|         |         | New     | to "Add | .aui-   |         | .aui-   |
|         |         | A       | New     | lozenge |         | lozenge |
|         |         | ddress" | C       | .aui-lo |         | .aui-lo |
|         |         |         | ontact" | zenge-s |         | zenge-s |
|         |         |         | page    | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-24 |         | Enter   | Shows a | [PASS]  |         | [YES]   |
|         |         | valid   | message | {.statu |         | {.statu |
|         |         | ad      | saying  | s-macro |         | s-macro |
|         |         | dress,\ | name is | .aui-   |         | .aui-   |
|         |         | Leave   | r       | lozenge |         | lozenge |
|         |         | name    | equired | .aui-lo |         | .aui-lo |
|         |         | empty   |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-25 |         | Enter   | Show an | [PASS]  |         | [YES]   |
|         |         | name,\  | error   | {.statu |         | {.statu |
|         |         | Enter   | (re     | s-macro |         | s-macro |
|         |         | invalid | cipient | .aui-   |         | .aui-   |
|         |         | address | address | lozenge |         | lozenge |
|         |         |         | network | .aui-lo |         | .aui-lo |
|         |         |         | unsup   | zenge-s |         | zenge-s |
|         |         |         | ported) | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-26 |         | Enter   | Shows a | [PASS]  |         | [YES]   |
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
| MENU-27 |         | Enter   | Shows a | [PASS]  |         | [YES]   |
|         |         | an      | message | {.statu |         | {.statu |
|         |         | address | saying  | s-macro |         | s-macro |
|         |         | that    | the     | .aui-   |         | .aui-   |
|         |         | already | address | lozenge |         | lozenge |
|         |         | exists  | exists  | .aui-lo |         | .aui-lo |
|         |         | in the  | in the  | zenge-s |         | zenge-s |
|         |         | wallet  | wallet  | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-28 |         | Enter   | New     | [PASS]  |         | [YES]   |
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
| MENU-29 | Custom  | Enter   | Enter   | [PASS]  |         | [YES]   |
|         |         | name,\  | custom  | {.statu |         | {.statu |
|         |         | Enter   | group   | s-macro |         | s-macro |
|         |         | valid   | name    | .aui-   |         | .aui-   |
|         |         | ad      | pop up  | lozenge |         | lozenge |
|         |         | dress,\ | is      | .aui-lo |         | .aui-lo |
|         |         | Choose  | shown   | zenge-s |         | zenge-s |
|         |         | custom  |         | uccess} |         | uccess} |
|         |         | group   |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-30 |         | Enter   | New     | [PASS]  |         | [YES]   |
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
| MENU-31 | Edit    | Click   | User    | [PASS]  |         | [YES]   |
|         | address | on edit | d       | {.statu |         | {.statu |
|         |         | address | irected | s-macro |         | s-macro |
|         |         |         | to edit | .aui-   |         | .aui-   |
|         |         |         | contact | lozenge |         | lozenge |
|         |         |         | page    | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-32 |         | Edit    | Show an | [PASS]  |         | [YES]   |
|         |         | name    | error   | {.statu |         | {.statu |
|         |         | field   |         | s-macro |         | s-macro |
|         |         | to be   |         | .aui-   |         | .aui-   |
|         |         | empty   |         | lozenge |         | lozenge |
|         |         |         |         | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-33 |         | Edit    | Show an | [PASS]  |         | [YES]   |
|         |         | address | error   | {.statu |         | {.statu |
|         |         | to be   |         | s-macro |         | s-macro |
|         |         | invalid |         | .aui-   |         | .aui-   |
|         |         |         |         | lozenge |         | lozenge |
|         |         |         |         | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-34 |         | Edit    | A       | [PASS]  |         | [YES]   |
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
| MENU-35 | Remove  | Click   | Prompts | [PASS]  |         | [YES]   |
|         | address | on      | for     | {.statu |         | {.statu |
|         |         | remove  | user    | s-macro |         | s-macro |
|         |         | address | confi   | .aui-   |         | .aui-   |
|         |         |         | rmation | lozenge |         | lozenge |
|         |         |         |         | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-36 |         | Click   | Contact | [PASS]  |         | [YES]   |
|         |         | remove  | is      | {.statu |         | {.statu |
|         |         | contact | removed | s-macro |         | s-macro |
|         |         |         | from    | .aui-   |         | .aui-   |
|         |         |         | address | lozenge |         | lozenge |
|         |         |         | book    | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-37 | Import  | Click   | Prompts | [PASS]  |         | [YES]   |
|         | Contact | on      | for     | {.statu |         | {.statu |
|         |         | import  | user to | s-macro |         | s-macro |
|         |         | tab,    | choose  | .aui-   |         | .aui-   |
|         |         | click   | file to | lozenge |         | lozenge |
|         |         | import  | add     | .aui-lo |         | .aui-lo |
|         |         | button  | contact | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-38 | Export  | Click   | Contact | [PASS]  |         |         |
|         | Contact | on      | is      | {.statu |         |         |
|         |         | export  | dow     | s-macro |         |         |
|         |         | tab,    | nloaded | .aui-   |         |         |
|         |         | click   | to      | lozenge |         |         |
|         |         | export  | user's  | .aui-lo |         |         |
|         |         | button  | local   | zenge-s |         |         |
|         |         |         | machine | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| MENU-39 | Sign    | Click   | Go back | [PASS]  |         | [YES]   |
|         | Out     | on      | to Sign | {.statu |         | {.statu |
|         |         | "Sign   | In page | s-macro |         | s-macro |
|         |         | Out"    |         | .aui-   |         | .aui-   |
|         |         | button  |         | lozenge |         | lozenge |
|         |         |         |         | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
|         |         |         |         |         |         | (under  |
|         |         |         |         |         |         | sign in |
|         |         |         |         |         |         | test)   |
+---------+---------+---------+---------+---------+---------+---------+
:::

::: table-wrap
+---------+---------+---------+---------+---------+---------+---------+
| #       |         |         |         |         |         |         |
| # Trans |         |         |         |         |         |         |
| fer (Ne |         |         |         |         |         |         |
| w Desig |         |         |         |         |         |         |
| n) {#Te |         |         |         |         |         |         |
| stCases |         |         |         |         |         |         |
| -0.0.10 |         |         |         |         |         |         |
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
|         |         | ransfer | list of | s-macro |         | s-macro |
|         |         | from    | a       | .aui-   |         | .aui-   |
|         |         | account | ccounts | lozenge |         | lozenge |
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
|         |         | address |         | .aui-   |         | .aui-   |
|         |         |         |         | lozenge |         | lozenge |
|         |         |         |         | .aui-lo |         | .aui-lo |
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
| TSFR-5  | T       | Leave   | Could   | [FAIL]  | User    | \-      |
|         | ransfer | t       | not     | {.statu | can     |         |
|         | amount  | ransfer | proceed | s-macro | still   |         |
|         |         | amount  | and     | .aui-   | proceed |         |
|         |         | as 0    | t       | lozenge | with    |         |
|         |         |         | ransfer | .aui-   | tran    |         |
|         |         |         | button  | lozenge | saction |         |
|         |         |         | is      | -error} |         |         |
|         |         |         | d       |         |         |         |
|         |         |         | isabled |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-6  | Message | Enter   | Tran    | [PASS]  |         | \-      |
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
| TSFR-7  |         | Enter   | P       | [FAIL]  | User    | \-      |
|         |         | more    | revents | {.statu | can     |         |
|         |         | than    | input   | s-macro | still   |         |
|         |         | maximum | upon    | .aui-   | input   |         |
|         |         | of      | r       | lozenge | message |         |
|         |         | message | eaching | .aui-   | ex      |         |
|         |         | limit   | maximum | lozenge | ceeding |         |
|         |         |         | message | -error} | the     |         |
|         |         |         | limit   |         | limit   |         |
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
| ##      |         |         |         |         |         |         |
|  Transf |         |         |         |         |         |         |
| er (Not |         |         |         |         |         |         |
|  applic |         |         |         |         |         |         |
| able fo |         |         |         |         |         |         |
| r now)  |         |         |         |         |         |         |
| {#TestC |         |         |         |         |         |         |
| ases-0. |         |         |         |         |         |         |
| 0.10-Tr |         |         |         |         |         |         |
| ansfer( |         |         |         |         |         |         |
| Notappl |         |         |         |         |         |         |
| icablef |         |         |         |         |         |         |
| ornow)} |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| **Test  | **Test  | **Test  | **E     | **S     | **R     | **Auto  |
| Case    | Scen    | steps** | xpected | tatus** | emark** | mated** |
| ID**    | arios** |         | r       |         |         |         |
|         |         |         | esult** |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-1  | Sender  | Observe | Default | [PASS]  |         |         |
|         | account | default | account | {.statu |         |         |
|         |         | value   | is      | s-macro |         |         |
|         |         | of      | being   | .aui-   |         |         |
|         |         | sender  | s       | lozenge |         |         |
|         |         | account | elected | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-2  |         | Check   | M       | [PASS]  |         |         |
|         |         | if      | ultisig | {.statu |         |         |
|         |         | m       | account | s-macro |         |         |
|         |         | ultisig | is      | .aui-   |         |         |
|         |         | account | shown   | lozenge |         |         |
|         |         | is      | on drop | .aui-lo |         |         |
|         |         | shown   | down    | zenge-s |         |         |
|         |         | on drop | list    | uccess} |         |         |
|         |         | down    |         |         |         |         |
|         |         | list    |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-3  |         | Check   | D       | [NOT    |         |         |
|         |         | if      | elegate | READY]  |         |         |
|         |         | d       | account | {.statu |         |         |
|         |         | elegate | is not  | s-macro |         |         |
|         |         | account | shown   | .aui-l  |         |         |
|         |         | is      | on drop | ozenge} |         |         |
|         |         | shown   | down    |         |         |         |
|         |         | on drop | list    |         |         |         |
|         |         | down    |         |         |         |         |
|         |         | list    |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-4  |         | Select  | C       | [PASS]  |         |         |
|         |         | m       | osigner | {.statu |         |         |
|         |         | ultisig | name    | s-macro |         |         |
|         |         | account | and     | .aui-   |         |         |
|         |         | which   | balance | lozenge |         |         |
|         |         | its     | is      | .aui-lo |         |         |
|         |         | c       | shown   | zenge-s |         |         |
|         |         | osigner | below   | uccess} |         |         |
|         |         | is in   |         |         |         |         |
|         |         | this    |         |         |         |         |
|         |         | wallet  |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-5  |         | If      | Shows   | [FAIL]  | Does    |         |
|         |         | cos     | insuf   | {.statu | not     |         |
|         |         | igner's | ficient | s-macro | show    |         |
|         |         | balance | balance | .aui-   | error   |         |
|         |         | is      | error   | lozenge |         |         |
|         |         | lower   |         | .aui-   |         |         |
|         |         | than    |         | lozenge |         |         |
|         |         | lock    |         | -error} |         |         |
|         |         | fund    |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-6  |         | Select  | No      | [PASS]  |         |         |
|         |         | m       | e       | {.statu |         |         |
|         |         | ultisig | ligible | s-macro |         |         |
|         |         | account | c       | .aui-   |         |         |
|         |         | which   | osigner | lozenge |         |         |
|         |         | its     | error   | .aui-lo |         |         |
|         |         | c       | is      | zenge-s |         |         |
|         |         | osigner | shown   | uccess} |         |         |
|         |         | is not  |         |         |         |         |
|         |         | in this |         |         |         |         |
|         |         | wallet  |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-7  | Re      | Enter   | Show a  | [PASS]  |         |         |
|         | cipient | invalid | message | {.statu |         |         |
|         |         | value   | "       | s-macro |         |         |
|         |         | on      | Invalid | .aui-   |         |         |
|         |         | re      | rec     | lozenge |         |         |
|         |         | cipient | ipient" | .aui-lo |         |         |
|         |         | field   |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-8  |         | Click   | A drop  | [PASS]  |         |         |
|         |         | on      | down    | {.statu |         |         |
|         |         | "Co     | list of | s-macro |         |         |
|         |         | ntact\" | c       | .aui-   |         |         |
|         |         | icon    | ontacts | lozenge |         |         |
|         |         |         | is      | .aui-lo |         |         |
|         |         |         | shown   | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-9  |         | Click   | Drop    | [PASS]  |         |         |
|         |         | on      | down    | {.statu |         |         |
|         |         | "C      | contact | s-macro |         |         |
|         |         | ontact" | list is | .aui-   |         |         |
|         |         | icon    | hidden  | lozenge |         |         |
|         |         | again   |         | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-10 |         | Click   | Owner's | [PASS]  |         |         |
|         |         | on      | normal  | {.statu |         |         |
|         |         | Contact | ac      | s-macro |         |         |
|         |         | drop    | counts, | .aui-   |         |         |
|         |         | down    | m       | lozenge |         |         |
|         |         | list    | ultisig | .aui-lo |         |         |
|         |         |         | a       | zenge-s |         |         |
|         |         |         | ccounts | uccess} |         |         |
|         |         |         | and     |         |         |         |
|         |         |         | c       |         |         |         |
|         |         |         | ontacts |         |         |         |
|         |         |         | are     |         |         |         |
|         |         |         | shown   |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-11 | XPX     | Enter   | Shows   | [FAIL]  | Shows 0 |         |
|         | amount  | invalid | NaN     | {.statu | instead |         |
|         |         | value   |         | s-macro |         |         |
|         |         |         |         | .aui-   |         |         |
|         |         |         |         | lozenge |         |         |
|         |         |         |         | .aui-   |         |         |
|         |         |         |         | lozenge |         |         |
|         |         |         |         | -error} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-12 |         | Balance | Shows   | [PASS]  |         |         |
|         |         | is less | insuf   | {.statu |         |         |
|         |         | than    | ficient | s-macro |         |         |
|         |         | tran    | balance | .aui-   |         |         |
|         |         | saction | error   | lozenge |         |         |
|         |         | fee     |         | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-13 |         | Entered | Shows   | [PASS]  |         |         |
|         |         | amount  | insuf   | {.statu |         |         |
|         |         | is more | ficient | s-macro |         |         |
|         |         | than    | balance | .aui-   |         |         |
|         |         | s       | error   | lozenge |         |         |
|         |         | elected |         | .aui-lo |         |         |
|         |         | account |         | zenge-s |         |         |
|         |         | balance |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-14 | Add     | Click   | Mosaic  | [PASS]  |         |         |
|         | Mosaics | "Add    | drop    | {.statu |         |         |
|         |         | M       | down    | s-macro |         |         |
|         |         | osaics" | list is | .aui-   |         |         |
|         |         |         | shown   | lozenge |         |         |
|         |         |         |         | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-15 |         | Select  | Shows   | [PASS]  |         |         |
|         |         | mosaic  | asset   | {.statu |         |         |
|         |         |         | id and  | s-macro |         |         |
|         |         |         | corres  | .aui-   |         |         |
|         |         |         | ponding | lozenge |         |         |
|         |         |         | balance | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-16 | Mosaic  | Entered | Shows   | [FAIL]  | Error   |         |
|         | amount  | amount  | insuf   | {.statu | message |         |
|         |         | is more | ficient | s-macro | not     |         |
|         |         | than    | balance | .aui-   | shown   |         |
|         |         | s       | error   | lozenge |         |         |
|         |         | elected |         | .aui-   |         |         |
|         |         | mosaic  |         | lozenge |         |         |
|         |         | balance |         | -error} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-17 | Regular | Click   | Works   | [PASS]  |         |         |
|         | /       | on both | p       | {.statu |         |         |
|         | Hexa    | radio   | roperly | s-macro |         |         |
|         | decimal | buttons |         | .aui-   |         |         |
|         |         |         |         | lozenge |         |         |
|         |         |         |         | .aui-lo |         |         |
|         |         |         |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-18 |         | Enter   | Allow   | [PASS]  |         |         |
|         |         | message | all     | {.statu |         |         |
|         |         | when    | inputs  | s-macro |         |         |
|         |         | regular |         | .aui-   |         |         |
|         |         | is      |         | lozenge |         |         |
|         |         | s       |         | .aui-lo |         |         |
|         |         | elected |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-19 |         | Enter   | Only    | [FAIL]  | Allows  |         |
|         |         | message | allow   | {.statu | all     |         |
|         |         | when    | hexa    | s-macro | inputs  |         |
|         |         | hexa    | decimal | .aui-   |         |         |
|         |         | decimal | inputs  | lozenge |         |         |
|         |         | is      |         | .aui-   |         |         |
|         |         | s       |         | lozenge |         |         |
|         |         | elected |         | -error} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-20 | En      | Click   | Works   | [NOT    |         |         |
|         | crypted | on      | p       | READY]  |         |         |
|         |         | c       | roperly | {.statu |         |         |
|         |         | heckbox |         | s-macro |         |         |
|         |         |         |         | .aui-l  |         |         |
|         |         |         |         | ozenge} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-21 | Message | Enter   | Ef      | [PASS]  |         |         |
|         |         | random  | fective | {.statu |         |         |
|         |         | m       | Fee     | s-macro |         |         |
|         |         | essages | in      | .aui-   |         |         |
|         |         |         | creases | lozenge |         |         |
|         |         |         | as      | .aui-lo |         |         |
|         |         |         | message | zenge-s |         |         |
|         |         |         | size    | uccess} |         |         |
|         |         |         | in      |         |         |         |
|         |         |         | creases |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-22 |         | Enter   | P       | [FAIL]  | User    |         |
|         |         | more    | revents | {.statu | can     |         |
|         |         | than    | input   | s-macro | still   |         |
|         |         | maximum | upon    | .aui-   | input   |         |
|         |         | of      | r       | lozenge | message |         |
|         |         | message | eaching | .aui-   | ex      |         |
|         |         | limit   | maximum | lozenge | ceeding |         |
|         |         |         | message | -error} | the     |         |
|         |         |         | limit   |         | limit   |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-23 | P       | Leave   | D       | [PASS]  |         |         |
|         | assword | p       | isplays | {.statu |         |         |
|         |         | assword | please  | s-macro |         |         |
|         |         | empty   | enter   | .aui-   |         |         |
|         |         |         | wallet  | lozenge |         |         |
|         |         |         | p       | .aui-lo |         |         |
|         |         |         | assword | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-24 | Clear   | Click   | Sender, | [PASS]  |         |         |
|         |         | on      | rec     | {.statu |         |         |
|         |         | clear   | ipient, | s-macro |         |         |
|         |         |         | send    | .aui-   |         |         |
|         |         |         | amount, | lozenge |         |         |
|         |         |         | mosaic  | .aui-lo |         |         |
|         |         |         | amount, | zenge-s |         |         |
|         |         |         | message | uccess} |         |         |
|         |         |         | and     |         |         |         |
|         |         |         | p       |         |         |         |
|         |         |         | assword |         |         |         |
|         |         |         | fields  |         |         |         |
|         |         |         | reset   |         |         |         |
|         |         |         | to      |         |         |         |
|         |         |         | default |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-25 | Create  | Click   | T       | [PASS]  |         |         |
|         |         | create  | ransfer | {.statu |         |         |
|         |         | when    | tran    | s-macro |         |         |
|         |         | there   | saction | .aui-   |         |         |
|         |         | are at  | is      | lozenge |         |         |
|         |         | least   | succe   | .aui-lo |         |         |
|         |         | re      | ssfully | zenge-s |         |         |
|         |         | cipient | created | uccess} |         |         |
|         |         | and     |         |         |         |         |
|         |         | p       |         |         |         |         |
|         |         | assword |         |         |         |         |
|         |         | field   |         |         |         |         |
|         |         | filled  |         |         |         |         |
|         |         | in      |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-26 |         | Click   | Create  | [PASS]  |         |         |
|         |         | create  | button  | {.statu |         |         |
|         |         | when    | is      | s-macro |         |         |
|         |         | any of  | d       | .aui-   |         |         |
|         |         | the     | isabled | lozenge |         |         |
|         |         | above   |         | .aui-lo |         |         |
|         |         | fields  |         | zenge-s |         |         |
|         |         | are     |         | uccess} |         |         |
|         |         | empty   |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-27 |         | Create  | T       | [NOT    |         |         |
|         |         | t       | ransfer | READY]  |         |         |
|         |         | ransfer | tran    | {.statu |         |         |
|         |         | with    | saction | s-macro |         |         |
|         |         | m       | is      | .aui-l  |         |         |
|         |         | ultisig | succe   | ozenge} |         |         |
|         |         | account | ssfully |         |         |         |
|         |         |         | created |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-28 |         | Create  | T       | [PASS]  |         |         |
|         |         | t       | ransfer | {.statu |         |         |
|         |         | ransfer | tran    | s-macro |         |         |
|         |         | with    | saction | .aui-   |         |         |
|         |         | normal  | is      | lozenge |         |         |
|         |         | account | succe   | .aui-lo |         |         |
|         |         |         | ssfully | zenge-s |         |         |
|         |         |         | created | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| TSFR-29 |         | Create  | Shows   | [PASS]  |         |         |
|         |         | any     | p       | {.statu |         |         |
|         |         | t       | assword | s-macro |         |         |
|         |         | ransfer | invalid | .aui-   |         |         |
|         |         | with    | error   | lozenge |         |         |
|         |         | wrong   |         | .aui-lo |         |         |
|         |         | p       |         | zenge-s |         |         |
|         |         | assword |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
:::

::: table-wrap
+---------+---------+---------+---------+---------+---------+---------+
| ## Ac   |         |         |         |         |         |         |
| counts  |         |         |         |         |         |         |
| {#TestC |         |         |         |         |         |         |
| ases-0. |         |         |         |         |         |         |
| 0.10-Ac |         |         |         |         |         |         |
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
|         |         | ccount" | Select  | lozenge |         | lozenge |
|         |         |         | C       | .aui-lo |         | .aui-lo |
|         |         |         | reation | zenge-s |         | zenge-s |
|         |         |         | Type"   | uccess} |         | uccess} |
|         |         |         | Page    |         |         |         |
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
| ACCTS-3 | Make as |         |         | [NOT    |         | \-      |
|         | Default |         |         | READY]  |         |         |
|         |         |         |         | {.statu |         |         |
|         |         |         |         | s-macro |         |         |
|         |         |         |         | .aui-l  |         |         |
|         |         |         |         | ozenge} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ACCTS-4 | Export  |         |         | [NOT    |         | \-      |
|         | Account |         |         | READY]  |         |         |
|         |         |         |         | {.statu |         |         |
|         |         |         |         | s-macro |         |         |
|         |         |         |         | .aui-l  |         |         |
|         |         |         |         | ozenge} |         |         |
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
| A       | T       | Click   | User is | [PASS]  |         | [YES]   |
| CCTS-10 | ransfer | on      | na      | {.statu |         | {.statu |
|         | XPX     | "T      | vigated | s-macro |         | s-macro |
|         |         | ransfer | to      | .aui-   |         | .aui-   |
|         |         | XPX"    | create  | lozenge |         | lozenge |
|         |         | button  | t       | .aui-lo |         | .aui-lo |
|         |         |         | ransfer | zenge-s |         | zenge-s |
|         |         |         | page    | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| A       | Request | Click   |         | [NOT    |         | \-      |
| CCTS-11 | XPX     | on      |         | READY]  |         |         |
|         |         | "       |         | {.statu |         |         |
|         |         | Request |         | s-macro |         |         |
|         |         | XPX"    |         | .aui-l  |         |         |
|         |         | button  |         | ozenge} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| A       | Top up  | Click   |         | [NOT    |         | \-      |
| CCTS-12 | XPX     | on "Top |         | READY]  |         |         |
|         |         | up XPX" |         | {.statu |         |         |
|         |         | button  |         | s-macro |         |         |
|         |         |         |         | .aui-l  |         |         |
|         |         |         |         | ozenge} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| A       | Restr   |         |         | [NOT    |         | \-      |
| CCTS-13 | ictions |         |         | READY]  |         |         |
|         |         |         |         | {.statu |         |         |
|         |         |         |         | s-macro |         |         |
|         |         |         |         | .aui-l  |         |         |
|         |         |         |         | ozenge} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| A       | M       |         |         | [NOT    |         | \-      |
| CCTS-14 | etadata |         |         | READY]  |         |         |
|         |         |         |         | {.statu |         |         |
|         |         |         |         | s-macro |         |         |
|         |         |         |         | .aui-l  |         |         |
|         |         |         |         | ozenge} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| A       | D       | Go to   | Account | [NOT    |         | \-      |
| CCTS-15 | elegate | "A      | is      | READY]  |         |         |
|         |         | ccounts | linked  | {.statu |         |         |
|         |         | \>      | to a    | s-macro |         |         |
|         |         | Del     | de      | .aui-l  |         |         |
|         |         | egate"\ | legated | ozenge} |         |         |
|         |         | Select  | a       |         |         |         |
|         |         | a       | ccount\ |         |         |         |
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
| A       |         | Click   | De      | [NOT    |         | \-      |
| CCTS-16 |         | "Save   | legated | READY]  |         |         |
|         |         | as      | ac      | {.statu |         |         |
|         |         | Wallet  | count's | s-macro |         |         |
|         |         | Paper"  | wallet  | .aui-l  |         |         |
|         |         | button  | paper   | ozenge} |         |         |
|         |         |         | dow     |         |         |         |
|         |         |         | nloaded |         |         |         |
|         |         |         | to      |         |         |         |
|         |         |         | user's  |         |         |         |
|         |         |         | local   |         |         |         |
|         |         |         | machine |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| A       |         | Click   | Go back | [NOT    |         | \-      |
| CCTS-17 |         | "C      | to      | READY]  |         |         |
|         |         | ontinue | A       | {.statu |         |         |
|         |         |         | ccounts | s-macro |         |         |
|         |         |         | \> View | .aui-l  |         |         |
|         |         |         | All     | ozenge} |         |         |
|         |         |         | page    |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ### Sel |         |         |         |         |         |         |
| ect Cre |         |         |         |         |         |         |
| ation T |         |         |         |         |         |         |
| ype {#T |         |         |         |         |         |         |
| estCase |         |         |         |         |         |         |
| s-0.0.1 |         |         |         |         |         |         |
| 0-Selec |         |         |         |         |         |         |
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
| #### C  |         |         |         |         |         |         |
| reate a |         |         |         |         |         |         |
|  New Ac |         |         |         |         |         |         |
| count i |         |         |         |         |         |         |
| n the s |         |         |         |         |         |         |
| ame Wal |         |         |         |         |         |         |
| let {#T |         |         |         |         |         |         |
| estCase |         |         |         |         |         |         |
| s-0.0.1 |         |         |         |         |         |         |
| 0-Creat |         |         |         |         |         |         |
| eaNewAc |         |         |         |         |         |         |
| countin |         |         |         |         |         |         |
| thesame |         |         |         |         |         |         |
| Wallet} |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| N       | Create  | Cu      | Go to   | [NOT    |         | \-      |
| EWACC-3 | a New   | rrently | "Select | READY]  |         |         |
|         | Account | in      | C       | {.statu |         |         |
|         |         | "Create | reation | s-macro |         |         |
|         |         | New     | Type"   | .aui-l  |         |         |
|         |         | A       |         | ozenge} |         |         |
|         |         | ccount" |         |         |         |         |
|         |         | page    |         |         |         |         |
|         |         | and     |         |         |         |         |
|         |         | click   |         |         |         |         |
|         |         | "Back"  |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| N       |         | Leave   | Show a  | [PASS]  |         | [YES]   |
| EWACC-4 |         | account | message | {.statu |         | {.statu |
|         |         | name    | "Enter  | s-macro |         | s-macro |
|         |         | empty   | Wallet  | .aui-   |         | .aui-   |
|         |         |         | Name"   | lozenge |         | lozenge |
|         |         |         |         | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| N       |         | Enter   | Show a  | [PASS]  |         | [YES]   |
| EWACC-5 |         | Account | message | {.statu |         | {.statu |
|         |         | Name,\  | "min    | s-macro |         | s-macro |
|         |         | Leave   | length  | .aui-   |         | .aui-   |
|         |         | p       | 8, max  | lozenge |         | lozenge |
|         |         | assword | length  | .aui-lo |         | .aui-lo |
|         |         | field   | 30",    | zenge-s |         | zenge-s |
|         |         | empty   | unable  | uccess} |         | uccess} |
|         |         |         | to      |         |         |         |
|         |         |         | create  |         |         |         |
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
| N       | Clear   | Enter   | Form is | [NOT    |         | \-      |
| EWACC-8 |         | Account | cleared | READY]  |         |         |
|         |         | Name,\  |         | {.statu |         |         |
|         |         | Enter   |         | s-macro |         |         |
|         |         | Correct |         | .aui-l  |         |         |
|         |         | Wallet  |         | ozenge} |         |         |
|         |         | Pa      |         |         |         |         |
|         |         | ssword\ |         |         |         |         |
|         |         | Click   |         |         |         |         |
|         |         | "Clear" |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| N       | Eye     | Click   | Sh      | [PASS]  |         | [YES]   |
| EWACC-9 | icon    | on      | ow/hide | {.statu |         | {.statu |
|         |         | "Pa     | p       | s-macro |         | s-macro |
|         |         | ssword" | assword | .aui-   |         | .aui-   |
|         |         | eye     |         | lozenge |         | lozenge |
|         |         | icon    |         | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| ##      |         |         |         |         |         |         |
| ## Crea |         |         |         |         |         |         |
| te a Ne |         |         |         |         |         |         |
| w Accou |         |         |         |         |         |         |
| nt from |         |         |         |         |         |         |
|  Privat |         |         |         |         |         |         |
| e Key i |         |         |         |         |         |         |
| n the s |         |         |         |         |         |         |
| ame Wal |         |         |         |         |         |         |
| let {#T |         |         |         |         |         |         |
| estCase |         |         |         |         |         |         |
| s-0.0.1 |         |         |         |         |         |         |
| 0-Creat |         |         |         |         |         |         |
| eaNewAc |         |         |         |         |         |         |
| countfr |         |         |         |         |         |         |
| omPriva |         |         |         |         |         |         |
| teKeyin |         |         |         |         |         |         |
| thesame |         |         |         |         |         |         |
| Wallet} |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      | Create  | Cu      | Go to   | [NOT    |         | \-      |
| WACC-10 | a New   | rrently | "Select | READY]  |         |         |
|         | Account | in      | C       | {.statu |         |         |
|         | from    | "Create | reation | s-macro |         |         |
|         | Private | New     | Type"   | .aui-l  |         |         |
|         | Key     | Account |         | ozenge} |         |         |
|         |         | From    |         |         |         |         |
|         |         | Private |         |         |         |         |
|         |         | Key"    |         |         |         |         |
|         |         | page    |         |         |         |         |
|         |         | and     |         |         |         |         |
|         |         | click   |         |         |         |         |
|         |         | "Back"  |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Leave   | Show a  | [PASS]  |         | [YES]   |
| WACC-11 |         | Private | message | {.statu |         | {.statu |
|         |         | Key     | "       | s-macro |         | s-macro |
|         |         | empty   | Invalid | .aui-   |         | .aui-   |
|         |         |         | Private | lozenge |         | lozenge |
|         |         |         | Key"    | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Enter   | Show a  | [PASS]  |         | [YES]   |
| WACC-12 |         | Private | message | {.statu |         | {.statu |
|         |         | Key,\   | "Enter  | s-macro |         | s-macro |
|         |         | Leave   | Wallet  | .aui-   |         | .aui-   |
|         |         | Account | Name"   | lozenge |         | lozenge |
|         |         | Name    |         | .aui-lo |         | .aui-lo |
|         |         | empty   |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| NE      |         | Enter   | Show a  | [PASS]  |         | [YES]   |
| WACC-13 |         | Private | message | {.statu |         | {.statu |
|         |         | Key,\   | "min    | s-macro |         | s-macro |
|         |         | Enter   | length  | .aui-   |         | .aui-   |
|         |         | Account | 8, max  | lozenge |         | lozenge |
|         |         | Name,\  | length  | .aui-lo |         | .aui-lo |
|         |         | Leave   | 30",    | zenge-s |         | zenge-s |
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
| WACC-14 |         | Private | message | {.statu |         | {.statu |
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
| WACC-15 |         | Private | confi   | {.statu |         | {.statu |
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
| NE      | Clear   | Enter   | Form is | [NOT    |         | \-      |
| WACC-16 |         | Private | cleared | READY]  |         |         |
|         |         | Key,\   |         | {.statu |         |         |
|         |         | Enter   |         | s-macro |         |         |
|         |         | Account |         | .aui-l  |         |         |
|         |         | Name,\  |         | ozenge} |         |         |
|         |         | Enter   |         |         |         |         |
|         |         | wallet  |         |         |         |         |
|         |         | pa      |         |         |         |         |
|         |         | ssword\ |         |         |         |         |
|         |         | Click   |         |         |         |         |
|         |         | "Clear" |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| NE      | Eye     | Click   | Sh      | [PASS]  |         | [YES]   |
| WACC-17 | icon    | on      | ow/hide | {.statu |         | {.statu |
|         |         | "Pa     | p       | s-macro |         | s-macro |
|         |         | ssword" | assword | .aui-   |         | .aui-   |
|         |         | eye     |         | lozenge |         | lozenge |
|         |         | icon    |         | .aui-lo |         | .aui-lo |
|         |         |         |         | zenge-s |         | zenge-s |
|         |         |         |         | uccess} |         | uccess} |
+---------+---------+---------+---------+---------+---------+---------+
| ### Edi |         |         |         |         |         |         |
| t an ex |         |         |         |         |         |         |
| isting  |         |         |         |         |         |         |
| Account |         |         |         |         |         |         |
|  {#Test |         |         |         |         |         |         |
| Cases-0 |         |         |         |         |         |         |
| .0.10-E |         |         |         |         |         |         |
| ditanex |         |         |         |         |         |         |
| istingA |         |         |         |         |         |         |
| ccount} |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ####    |         |         |         |         |         |         |
| Details |         |         |         |         |         |         |
|  {#Test |         |         |         |         |         |         |
| Cases-0 |         |         |         |         |         |         |
| .0.10-D |         |         |         |         |         |         |
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
|         |         | wallet  | "Please | s-macro |         | s-macro |
|         |         | pa      | insert  | .aui-   |         | .aui-   |
|         |         | ssword\ | wallet  | lozenge |         | lozenge |
|         |         | Click   | p       | .aui-lo |         | .aui-lo |
|         |         | "C      | assword | zenge-s |         | zenge-s |
|         |         | onfirm" | to show | uccess} |         | uccess} |
|         |         |         | Private |         |         |         |
|         |         |         | Key"    |         |         |         |
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
|         |         | wallet  | "Please | s-macro |         | s-macro |
|         |         | pa      | insert  | .aui-   |         | .aui-   |
|         |         | ssword\ | wallet  | lozenge |         | lozenge |
|         |         | Click   | p       | .aui-lo |         | .aui-lo |
|         |         | "C      | assword | zenge-s |         | zenge-s |
|         |         | onfirm" | to save | uccess} |         | uccess} |
|         |         |         | paper   |         |         |         |
|         |         |         | wallet" |         |         |         |
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
| ### C   |         |         |         |         |         |         |
| onvert  |         |         |         |         |         |         |
| to Mult |         |         |         |         |         |         |
| isig {# |         |         |         |         |         |         |
| TestCas |         |         |         |         |         |         |
| es-0.0. |         |         |         |         |         |         |
| 10-Conv |         |         |         |         |         |         |
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
| CVT     | Send    | Click   | C       | \-      |         | \-      |
| MTSG-11 |         | "Update | onverts |         |         |         |
|         |         | Cosigna | account |         |         |         |
|         |         | tories" | to      |         |         |         |
|         |         | when    | m       |         |         |         |
|         |         | there   | ultisig |         |         |         |
|         |         | is at   |         |         |         |         |
|         |         | least   |         |         |         |         |
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
| CVT     |         | Click   | Shows a | [PASS]  |         | [YES]   |
| MTSG-12 |         | "Update | message | {.statu |         | {.statu |
|         |         | Cosigna | "P      | s-macro |         | s-macro |
|         |         | tories" | assword | .aui-   |         | .aui-   |
|         |         | when    | for     | lozenge |         | lozenge |
|         |         | p       | wallet  | .aui-lo |         | .aui-lo |
|         |         | assword | \<name  | zenge-s |         | zenge-s |
|         |         | is      | of      | uccess} |         | uccess} |
|         |         | invalid | w       |         |         |         |
|         |         |         | allet\> |         |         |         |
|         |         |         | is      |         |         |         |
|         |         |         | i       |         |         |         |
|         |         |         | nvalid" |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| #       |         |         |         |         |         |         |
| ## Edit |         |         |         |         |         |         |
|  Multis |         |         |         |         |         |         |
| ig {#Te |         |         |         |         |         |         |
| stCases |         |         |         |         |         |         |
| -0.0.10 |         |         |         |         |         |         |
| -EditMu |         |         |         |         |         |         |
| ltisig} |         |         |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ED      | M       | Click   | M       | [NOT    |         | \-      |
| TMTSG-1 | ultisig | branch  | ultisig | READY]  |         |         |
|         | Graph   | icon    | graph   | {.statu |         |         |
|         |         |         | is      | s-macro |         |         |
|         |         |         | di      | .aui-l  |         |         |
|         |         |         | splayed | ozenge} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ED      | Remove  | Click   | Cosign  | [NOT    |         | \-      |
| TMTSG-2 | cosi    | on drop | atories | READY]  |         |         |
|         | gnatory | down    | are     | {.statu |         |         |
|         |         | icon    | di      | s-macro |         |         |
|         |         |         | splayed | .aui-l  |         |         |
|         |         |         |         | ozenge} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ED      |         | Click   | S       | [NOT    |         | \-      |
| TMTSG-3 |         | on      | elected | READY]  |         |         |
|         |         | delete  | c       | {.statu |         |         |
|         |         | icon    | osigner | s-macro |         |         |
|         |         |         | is      | .aui-l  |         |         |
|         |         |         | high    | ozenge} |         |         |
|         |         |         | lighted |         |         |         |
|         |         |         | as      |         |         |         |
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
| ED      | Scheme  | Add and | Value   | [PASS]  |         |         |
| TMTSG-7 |         | reduce  | does    | {.statu |         |         |
|         |         | approve | not     | s-macro |         |         |
|         |         | trans   | exceed  | .aui-   |         |         |
|         |         | actions | max     | lozenge |         |         |
|         |         |         | number  | .aui-lo |         |         |
|         |         |         | of      | zenge-s |         |         |
|         |         |         | cosign  | uccess} |         |         |
|         |         |         | atories |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| ED      |         | Add and | Value   | [PASS]  |         |         |
| TMTSG-8 |         | reduce  | does    | {.statu |         |         |
|         |         | delete  | not     | s-macro |         |         |
|         |         | users   | exceed  | .aui-   |         |         |
|         |         |         | max     | lozenge |         |         |
|         |         |         | number  | .aui-lo |         |         |
|         |         |         | of      | zenge-s |         |         |
|         |         |         | cosign  | uccess} |         |         |
|         |         |         | atories |         |         |         |
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
| EDT     | Clear   | Click   | Scheme, | [PASS]  |         |         |
| MTSG-12 |         | clear   | added   | {.statu |         |         |
|         |         |         | Cosig   | s-macro |         |         |
|         |         |         | natory, | .aui-   |         |         |
|         |         |         | r       | lozenge |         |         |
|         |         |         | emoving | .aui-lo |         |         |
|         |         |         | cosi    | zenge-s |         |         |
|         |         |         | gnatory | uccess} |         |         |
|         |         |         | and     |         |         |         |
|         |         |         | p       |         |         |         |
|         |         |         | assword |         |         |         |
|         |         |         | field   |         |         |         |
|         |         |         | are     |         |         |         |
|         |         |         | reset   |         |         |         |
|         |         |         | to      |         |         |         |
|         |         |         | default |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| EDT     | Send    | Click   | Edit    | [PASS]  |         |         |
| MTSG-13 |         | send    | m       | {.statu |         |         |
|         |         | when    | ultisig | s-macro |         |         |
|         |         | p       | account | .aui-   |         |         |
|         |         | assword |         | lozenge |         |         |
|         |         | field   |         | .aui-lo |         |         |
|         |         | is      |         | zenge-s |         |         |
|         |         | filled  |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| EDT     |         | Click   | Send    | [PASS]  |         |         |
| MTSG-14 |         | send    | button  | {.statu |         |         |
|         |         | when    | is      | s-macro |         |         |
|         |         | scheme  | d       | .aui-   |         |         |
|         |         | values  | isabled | lozenge |         |         |
|         |         | are     |         | .aui-lo |         |         |
|         |         | a       |         | zenge-s |         |         |
|         |         | djusted |         | uccess} |         |         |
|         |         | to 0    |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| EDT     |         | Click   | Send    | [PASS]  |         |         |
| MTSG-15 |         | send    | button  | {.statu |         |         |
|         |         | when    | is      | s-macro |         |         |
|         |         | any of  | d       | .aui-   |         |         |
|         |         | the     | isabled | lozenge |         |         |
|         |         | above   |         | .aui-lo |         |         |
|         |         | are not |         | zenge-s |         |         |
|         |         | fu      |         | uccess} |         |         |
|         |         | lfilled |         |         |         |         |
+---------+---------+---------+---------+---------+---------+---------+
| EDT     |         | Click   | D       | [PASS]  |         |         |
| MTSG-16 |         | send    | isplays | {.statu |         |         |
|         |         | when    | p       | s-macro |         |         |
|         |         | p       | assword | .aui-   |         |         |
|         |         | assword | invalid | lozenge |         |         |
|         |         | is      | error   | .aui-lo |         |         |
|         |         | invalid |         | zenge-s |         |         |
|         |         |         |         | uccess} |         |         |
+---------+---------+---------+---------+---------+---------+---------+
:::

## Services {#TestCases-0.0.10-Services}

### Namespaces {#TestCases-0.0.10-Namespaces}

#### Register {#TestCases-0.0.10-Register style="margin-left: 30.0px;"}

#### Extend Duration {#TestCases-0.0.10-ExtendDuration style="margin-left: 30.0px;"}

### Assets {#TestCases-0.0.10-Assets}

#### Create {#TestCases-0.0.10-Create style="margin-left: 30.0px;"}

#### Modify Supply {#TestCases-0.0.10-ModifySupply style="margin-left: 30.0px;"}

#### Link to Namespaces {#TestCases-0.0.10-LinktoNamespaces style="margin-left: 30.0px;"}

### Swap {#TestCases-0.0.10-Swap}

#### NIS1 {#TestCases-0.0.10-NIS1 style="margin-left: 30.0px;"}

#### ETH {#TestCases-0.0.10-ETH style="margin-left: 30.0px;"}

#### BSC {#TestCases-0.0.10-BSC style="margin-left: 30.0px;"}

### Address Book {#TestCases-0.0.10-AddressBook}

#### List {#TestCases-0.0.10-List style="margin-left: 30.0px;"}

#### Add Contacts {#TestCases-0.0.10-AddContacts style="margin-left: 30.0px;"}

### Wallets {#TestCases-0.0.10-Wallets}

#### Change Password {#TestCases-0.0.10-ChangePassword style="margin-left: 30.0px;"}

#### Export {#TestCases-0.0.10-Export style="margin-left: 30.0px;"}

#### Delete {#TestCases-0.0.10-Delete style="margin-left: 30.0px;"}

### Voting {#TestCases-0.0.10-Voting}

#### Create Poll {#TestCases-0.0.10-CreatePoll style="margin-left: 30.0px;"}

#### Vote {#TestCases-0.0.10-Vote style="margin-left: 30.0px;"}

#### View Results {#TestCases-0.0.10-ViewResults style="margin-left: 30.0px;"}

### Storage {#TestCases-0.0.10-Storage}

#### Files {#TestCases-0.0.10-Files style="margin-left: 30.0px;"}

#### Upload File {#TestCases-0.0.10-UploadFile style="margin-left: 30.0px;"}

#### Send/Share {#TestCases-0.0.10-Send/Share style="margin-left: 30.0px;"}

### Sirius Gift {#TestCases-0.0.10-SiriusGift}

#### Create {#TestCases-0.0.10-Create.1 style="margin-left: 30.0px;"}

#### Redeem {#TestCases-0.0.10-Redeem style="margin-left: 30.0px;"}

### Aggregate Transactions {#TestCases-0.0.10-AggregateTransactions}

#### Complete {#TestCases-0.0.10-Complete style="margin-left: 30.0px;"}

#### Bonded {#TestCases-0.0.10-Bonded style="margin-left: 30.0px;"}
:::

::: {.pageSection .group}
::: pageSectionHeader
## Attachments: {#attachments .pageSectionTitle}
:::

::: {.greybox align="left"}
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331639889)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331639900)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331639911)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331639922)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331639933)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331639944)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2334130278)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2334130289)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2334130300)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2334130311)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2334130322)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2334163006)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[JuJFRQviEuNr-LFhKKtzgok1mpF5HDikOIL1_xWg6aGr2qkQ8QSbxpffBmBBZjHP0mp8bWeQOwXRWRwlDCdz6gs25qus8boYnGvW4GVGSyi0cdVFcdwMCJyRp_oVci2AbNXYamEotatFLomrkg](attachments/2331672651/2331705454)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2334163017)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2334163028)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2334163039)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2334163056)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[-bO8lWnCxvS5X986IxWgckBxaJCAbxhYl3-TF3royi6Q4j9TP6fotHOWiQ-il3_ryQNouMJ4csO5ZSgD_ZjKbkejc_edkj4PbVtm6f83nPyVS5LMbxvR1CSNaPwQrwZqw6pPpu1WRhThCx6m3A](attachments/2331672651/2331705509)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2334163067)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2334163078)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2334163089)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2334163100)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2334163111)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2334163122)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2334163139)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[b6Y7vdCjGYj4Iz0F_WS65i2cmIOlSUT86qa6i_8b-nI5nMCdfPd8pzyZ7F00oJUCaExJm6trTRKlkKGVJ7Sk77IHaRM8J3xiPRDc7QBvZKdGSgTdYDf5PENJN1AGkDy16cx3ElRHYzDKpmmMJA](attachments/2331672651/2331705597)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2334163150)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2334163161)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2334163172)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2334163183)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331705465)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[JuJFRQviEuNr-LFhKKtzgok1mpF5HDikOIL1_xWg6aGr2qkQ8QSbxpffBmBBZjHP0mp8bWeQOwXRWRwlDCdz6gs25qus8boYnGvW4GVGSyi0cdVFcdwMCJyRp_oVci2AbNXYamEotatFLomrkg](attachments/2331672651/2334163000)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331705476)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331705487)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331705498)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331705520)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[-bO8lWnCxvS5X986IxWgckBxaJCAbxhYl3-TF3royi6Q4j9TP6fotHOWiQ-il3_ryQNouMJ4csO5ZSgD_ZjKbkejc_edkj4PbVtm6f83nPyVS5LMbxvR1CSNaPwQrwZqw6pPpu1WRhThCx6m3A](attachments/2331672651/2334163050)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331705531)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331705542)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331705553)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331705564)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331705575)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331705586)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331705608)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[b6Y7vdCjGYj4Iz0F_WS65i2cmIOlSUT86qa6i_8b-nI5nMCdfPd8pzyZ7F00oJUCaExJm6trTRKlkKGVJ7Sk77IHaRM8J3xiPRDc7QBvZKdGSgTdYDf5PENJN1AGkDy16cx3ElRHYzDKpmmMJA](attachments/2331672651/2334163133)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331705619)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331705630)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331705641)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331705652)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331607110)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331607121)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331607132)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331607143)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2335801348)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2335801359)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2335801370)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2335801381)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2335801392)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2335801403)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2335801414)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331640031)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331640042)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331640053)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331640064)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331640075)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2336129028)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2336129039)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2336129050)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2336129061)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2336129072)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2336129083)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2336129094)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331640091)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331640102)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331640113)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331640124)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331640135)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331640146)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331640157)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331640168)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331640179)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331640190)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331640201)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331640212)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331640223)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331640234)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331640245)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331640256)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331640267)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331640278)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331640289)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331640300)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331640311)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2336063494)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2336063505)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2336063516)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2336063527)
(image/png)\
![](images/icons/bullet_blue.gif){height="8" width="8"}
[IOJtLL0pqd1aniALXKyPdTwxaxYGSn3W1jljOpG7QSdSuVCpi_dPYNT7_TSWzywuHOToIQl_8CJ_Xcrub9PH6CVRPuiqvTt8-hr2133s6-CuwilYN9765uwm5vmiRFP8aSNp115F0eCwsraFrQ](attachments/2331672651/2331639883)
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
