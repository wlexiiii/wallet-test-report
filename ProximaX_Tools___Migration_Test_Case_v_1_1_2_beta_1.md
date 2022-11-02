::: {#page}
::: {#main .aui-page-panel}
::: {#main-header}
::: {#breadcrumb-section}
1.  [ProximaX Tools](index.html)
2.  [Test Reports](Test-Reports_2443871313.html)
:::

# [ ProximaX Tools : Migration Test Case v.1.1.2-beta-1 ]{#title-text} {#title-heading .pagetitle}
:::

::: {#content .view}
::: page-metadata
Created by [ davidwunarsa]{.author}, last modified by [ Shin
Neng]{.editor} on Apr 27, 2022
:::

::: {#main-content .wiki-content .group}
Date: 07/04/2022\
Version: 1.1.2-beta-1\
Test Environment: Mozilla Firefox (Version 98.0.2(64-bit)), Linux Ubuntu
20.04, Core i7-8750H CPU \@2.20GHz, 8GB RAM\
Staging Link: Local host - testnet 2\
Browser: Mozilla Firefox (Version 98.0.2(64-bit))\
Testnet: Testnet 2

Reviewer:

-   [[Shin
    Neng](https://nemspfs.atlassian.net/wiki/people/5b84fef69170df2b44b5ef67?ref=confluence){.confluence-userlink
    .user-mention username="5b84fef69170df2b44b5ef67"
    account-id="5b84fef69170df2b44b5ef67" target="_blank"
    linked-resource-id="86540290" linked-resource-version="1"
    linked-resource-type="userinfo"
    base-url="https://nemspfs.atlassian.net/wiki"} [
    [![](https://nemspfs.atlassian.net/rest/api/2/universal_avatar/view/type/issuetype/avatar/10318?size=medium){.icon}WLT-9](https://nemspfs.atlassian.net/browse/WLT-9){.jira-issue-key} -
    [Migration test case v1.1.2-beta review]{.summary}
    [Done]{.aui-lozenge .aui-lozenge-subtle .aui-lozenge-success
    .jira-macro-single-issue-export-pdf} ]{.confluence-jim-macro
    .jira-issue .resolved jira-key="WLT-9"} ]{.placeholder-inline-tasks}

::: table-wrap
+----------+----------+----------+----------+----------+----------+
| ## Old   |          |          |          |          |          |
| Wallet - |          |          |          |          |          |
|  Main Pa |          |          |          |          |          |
| ge {#Mig |          |          |          |          |          |
| rationTe |          |          |          |          |          |
| stCasev. |          |          |          |          |          |
| 1.1.2-be |          |          |          |          |          |
| ta-1-Old |          |          |          |          |          |
| Wallet-M |          |          |          |          |          |
| ainPage} |          |          |          |          |          |
+----------+----------+----------+----------+----------+----------+
| **Test   | **Test   | **Test   | **       | **       | **       |
| Case     | Sce      | steps**  | Expected | Status** | Remark** |
| ID**     | narios** |          | result** |          |          |
+----------+----------+----------+----------+----------+----------+
| OldM-1   | Sign in  | Select   | Unable   | [PAS     |          |
|          |          | wallet   | to sign  | S]{.stat |          |
|          |          | and      | in,      | us-macro |          |
|          |          | click on | "Sign    | .aui     |          |
|          |          | "Sign    | In"      | -lozenge |          |
|          |          | in"      | button   | .aui-    |          |
|          |          | button   | is       | lozenge- |          |
|          |          | without  | disabled | success} |          |
|          |          | entering |          |          |          |
|          |          | password |          |          |          |
+----------+----------+----------+----------+----------+----------+
| OldM-2   |          | Select   | Go to    | [PAS     |          |
|          |          | wallet,  | the main | S]{.stat |          |
|          |          | enter    | home     | us-macro |          |
|          |          | password | page of  | .aui     |          |
|          |          | and      | Sirius   | -lozenge |          |
|          |          | click on | Wallet   | .aui-    |          |
|          |          | "Sign    |          | lozenge- |          |
|          |          | in"      |          | success} |          |
|          |          | button   |          |          |          |
+----------+----------+----------+----------+----------+----------+
| OldM-3   |          | Enter    | Show an  | [PAS     |          |
|          |          | invalid  | error    | S]{.stat |          |
|          |          | password | message  | us-macro |          |
|          |          |          | "Invalid | .aui     |          |
|          |          |          | P        | -lozenge |          |
|          |          |          | assword" | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| OldM-4   | Create   | Click on | Go to    | [PAS     |          |
|          | New      | "Create  | screen   | S]{.stat |          |
|          | Account  | Account  | "Create  | us-macro |          |
|          | Wallet   | Wallet"  | Wallet"  | .aui     |          |
|          |          | button   | with 3   | -lozenge |          |
|          |          |          | s        | .aui-    |          |
|          |          |          | election | lozenge- |          |
|          |          |          | types    | success} |          |
|          |          |          | (new     |          |          |
|          |          |          | wallet,  |          |          |
|          |          |          | private  |          |          |
|          |          |          | key,     |          |          |
|          |          |          | wallet   |          |          |
|          |          |          | backup"  |          |          |
+----------+----------+----------+----------+----------+----------+
:::

::: table-wrap
+----------+----------+----------+----------+----------+----------+
| ## Old   |          |          |          |          |          |
|  Wallet  |          |          |          |          |          |
| - Create |          |          |          |          |          |
|  New Wal |          |          |          |          |          |
| let {#Mi |          |          |          |          |          |
| grationT |          |          |          |          |          |
| estCasev |          |          |          |          |          |
| .1.1.2-b |          |          |          |          |          |
| eta-1-Ol |          |          |          |          |          |
| dWallet- |          |          |          |          |          |
| CreateNe |          |          |          |          |          |
| wWallet} |          |          |          |          |          |
+----------+----------+----------+----------+----------+----------+
| **Test   | **Test   | **Test   | **       | **       | **       |
| Case     | Sce      | steps**  | Expected | Status** | Remark** |
| ID**     | narios** |          | result** |          |          |
+----------+----------+----------+----------+----------+----------+
| OLDWLT-1 | Create\  | Click on | Go to    | [PAS     |          |
|          | (New     | Create   | screen   | S]{.stat |          |
|          | Wallet)  | "New     | "Create  | us-macro |          |
|          |          | Wallet"  | Wallet " | .aui     |          |
|          |          | button   |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| OLDWLT-2 | Wallet   | Leave    | Show a   | [PAS     |          |
|          | name     | the      | message  | S]{.stat |          |
|          |          | field    | "Enter   | us-macro |          |
|          |          | empty    | Wallet   | .aui     |          |
|          |          |          | Name"    | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| OLDWLT-3 |          | Set      | Special  | [PAS     |          |
|          |          | special  | Ch       | S]{.stat |          |
|          |          | ch       | aracters | us-macro |          |
|          |          | aracters | can be   | .aui     |          |
|          |          |          | used     | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| OLDWLT-4 | P        | Leave    | Show an  | [PAS     |          |
|          | assword  | the      | error    | S]{.stat |          |
|          |          | field    | message  | us-macro |          |
|          |          | empty    |          | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| OLDWLT-5 |          | Set an   | Show a   | [PAS     |          |
|          |          | invalid  | message  | S]{.stat |          |
|          |          | password | "p       | us-macro |          |
|          |          |          | assword" | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| OLDWLT-6 |          | Set      | Special  | [PAS     |          |
|          |          | special  | Ch       | S]{.stat |          |
|          |          | ch       | aracters | us-macro |          |
|          |          | aracters | can be   | .aui     |          |
|          |          |          | used     | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| OLDWLT-7 |          | Place    | Show     | [PAS     |          |
|          |          | less     | message  | S]{.stat |          |
|          |          | than     | of       | us-macro |          |
|          |          | required | minimum  | .aui     |          |
|          |          | values   | ch       | -lozenge |          |
|          |          |          | aracters | .aui-    |          |
|          |          |          | to       | lozenge- |          |
|          |          |          | enter\   | success} |          |
|          |          |          | "min     |          |          |
|          |          |          | length   |          |          |
|          |          |          | 8"       |          |          |
+----------+----------+----------+----------+----------+----------+
| OLDWLT-8 | Confirm  | Leave    | Show a   | [PAS     |          |
|          | password | the      | message\ | S]{.stat |          |
|          |          | field    | "        | us-macro |          |
|          |          | empty    | Password | .aui     |          |
|          |          |          | doesn't  | -lozenge |          |
|          |          |          | match"   | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| OLDWLT-9 |          | Enter a  | Show a   | [PAS     |          |
|          |          | d        | message\ | S]{.stat |          |
|          |          | ifferent | "        | us-macro |          |
|          |          | password | Password | .aui     |          |
|          |          |          | doesn't  | -lozenge |          |
|          |          |          | match"   | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| O        |          | Set      | Special  | [PAS     |          |
| LDWLT-10 |          | special  | Ch       | S]{.stat |          |
|          |          | ch       | aracters | us-macro |          |
|          |          | aracters | can be   | .aui     |          |
|          |          |          | used     | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| O        |          | Place    | Show a   | [PAS     |          |
| LDWLT-11 |          | less or  | message\ | S]{.stat |          |
|          |          | more     | "        | us-macro |          |
|          |          | than     | Password | .aui     |          |
|          |          | required | doesn't  | -lozenge |          |
|          |          | values   | match"   | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| O        | Eye      | Click on | Show /   | [PAS     |          |
| LDWLT-12 | Icons    | "P       | hide the | S]{.stat |          |
|          |          | assword" | password | us-macro |          |
|          |          | eye icon |          | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| O        |          | Click on | Show /   | [PAS     |          |
| LDWLT-13 |          | "Confirm | hide the | S]{.stat |          |
|          |          | p        | password | us-macro |          |
|          |          | assword" |          | .aui     |          |
|          |          | eye icon |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| O        | Clear    | Click on | Clean    | [PAS     |          |
| LDWLT-14 |          | "Clear"  | the form | S]{.stat |          |
|          |          | button   |          | us-macro |          |
|          |          |          |          | .aui     |          |
|          |          |          |          | -lozenge |          |
|          |          |          |          | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| O        | Create   | Click on | Send a   | [PAS     |          |
| LDWLT-15 |          | "Create  | conf     | S]{.stat |          |
|          |          | Wallet"  | irmation | us-macro |          |
|          |          | button   | message  | .aui     |          |
|          |          |          | and      | -lozenge |          |
|          |          |          | create   | .aui-    |          |
|          |          |          | the      | lozenge- |          |
|          |          |          | wallet   | success} |          |
+----------+----------+----------+----------+----------+----------+
:::

::: table-wrap
+----------+----------+----------+----------+----------+----------+
| ##       |          |          |          |          |          |
|  New Wal |          |          |          |          |          |
| let - Im |          |          |          |          |          |
| porting  |          |          |          |          |          |
| Wallet f |          |          |          |          |          |
| rom Old  |          |          |          |          |          |
| Wallet { |          |          |          |          |          |
| #Migrati |          |          |          |          |          |
| onTestCa |          |          |          |          |          |
| sev.1.1. |          |          |          |          |          |
| 2-beta-1 |          |          |          |          |          |
| -NewWall |          |          |          |          |          |
| et-Impor |          |          |          |          |          |
| tingWall |          |          |          |          |          |
| etfromOl |          |          |          |          |          |
| dWallet} |          |          |          |          |          |
+----------+----------+----------+----------+----------+----------+
| **Test   | **Test   | **Test   | **       | **       | **       |
| Case     | Sce      | steps**  | Expected | Status** | Remark** |
| ID**     | narios** |          | result** |          |          |
+----------+----------+----------+----------+----------+----------+
| NEWWLT-1 | Sign in  | Select   | Unable   | [PAS     |          |
|          |          | wallet   | to sign  | S]{.stat |          |
|          |          | and      | in,      | us-macro |          |
|          |          | click on | "Sign    | .aui     |          |
|          |          | "Sign    | In"      | -lozenge |          |
|          |          | in"      | button   | .aui-    |          |
|          |          | button   | is       | lozenge- |          |
|          |          | without  | disabled | success} |          |
|          |          | entering |          |          |          |
|          |          | password |          |          |          |
+----------+----------+----------+----------+----------+----------+
| NEWWLT-2 |          | Select   | Go to    | [PAS     |          |
|          |          | wallet,  | the main | S]{.stat |          |
|          |          | enter    | home     | us-macro |          |
|          |          | password | page of  | .aui     |          |
|          |          | and      | Sirius   | -lozenge |          |
|          |          | click on | Wallet   | .aui-    |          |
|          |          | "Sign    |          | lozenge- |          |
|          |          | in"      |          | success} |          |
|          |          | button   |          |          |          |
+----------+----------+----------+----------+----------+----------+
| NEWWLT-3 |          | Enter    | Show an  | [PAS     |          |
|          |          | invalid  | error    | S]{.stat |          |
|          |          | password | message  | us-macro |          |
|          |          |          | "Invalid | .aui     |          |
|          |          |          | P        | -lozenge |          |
|          |          |          | assword" | .aui-    |          |
|          |          |          |          | lozenge- |          |
|          |          |          |          | success} |          |
+----------+----------+----------+----------+----------+----------+
| NEWWLT-4 | Backup   | Click on | All      | [PAS     |          |
|          | Old      | "Backup  | wallet   | S]{.stat |          |
|          | Wallet   | Old      | accounts | us-macro |          |
|          |          | Wallet"  | created  | .aui     |          |
|          |          |          | in old   | -lozenge |          |
|          |          |          | wallet   | .aui-    |          |
|          |          |          | is       | lozenge- |          |
|          |          |          | do       | success} |          |
|          |          |          | wnloaded |          |          |
|          |          |          | to local |          |          |
|          |          |          | machine  |          |          |
+----------+----------+----------+----------+----------+----------+
| NEWWLT-5 | Create   | Click on | Go to    | [PAS     |          |
|          | New      | "Create  | screen   | S]{.stat |          |
|          | Account  | Account  | "Create  | us-macro |          |
|          | Wallet   | Wallet"  | Wallet"  | .aui     |          |
|          |          | button   | with 3   | -lozenge |          |
|          |          |          | s        | .aui-    |          |
|          |          |          | election | lozenge- |          |
|          |          |          | types    | success} |          |
|          |          |          | (new     |          |          |
|          |          |          | wallet,  |          |          |
|          |          |          | private  |          |          |
|          |          |          | key,     |          |          |
|          |          |          | wallet   |          |          |
|          |          |          | backup"  |          |          |
+----------+----------+----------+----------+----------+----------+
| NEWWLT-6 |          | Click on | Go to    | [PAS     |          |
|          |          | "From a  | screen   | S]{.stat |          |
|          |          | Wallet   | "Create  | us-macro |          |
|          |          | Backup"  | Wallet   | .aui     |          |
|          |          | button   | from a   | -lozenge |          |
|          |          |          | Wallet   | .aui-    |          |
|          |          |          | Backup"  | lozenge- |          |
|          |          |          | and      | success} |          |
|          |          |          | import   |          |          |
|          |          |          | button   |          |          |
|          |          |          | a        |          |          |
|          |          |          | vailable |          |          |
|          |          |          | to       |          |          |
|          |          |          | browse   |          |          |
|          |          |          | for the  |          |          |
|          |          |          | .wlt     |          |          |
|          |          |          | file     |          |          |
+----------+----------+----------+----------+----------+----------+
| NEWWLT-7 |          | Click on | User     | [PAS     |          |
|          |          | "Import  | will be  | S]{.stat |          |
|          |          | File"    | prompted | us-macro |          |
|          |          | button   | to       | .aui     |          |
|          |          |          | browse   | -lozenge |          |
|          |          |          | for the  | .aui-    |          |
|          |          |          | .wlt     | lozenge- |          |
|          |          |          | file     | success} |          |
|          |          |          | that has |          |          |
|          |          |          | been     |          |          |
|          |          |          | do       |          |          |
|          |          |          | wnloaded |          |          |
|          |          |          | and old  |          |          |
|          |          |          | account  |          |          |
|          |          |          | will be  |          |          |
|          |          |          | succ     |          |          |
|          |          |          | essfully |          |          |
|          |          |          | created  |          |          |
|          |          |          | on the   |          |          |
|          |          |          | new      |          |          |
|          |          |          | wallet   |          |          |
+----------+----------+----------+----------+----------+----------+
| NEWWLT-8 | Sign in  | Select   | Go to    | [PAS     |          |
|          | with old | wallet,  | the main | S]{.stat |          |
|          | wallet   | enter    | home     | us-macro |          |
|          | account  | same     | page of  | .aui     |          |
|          |          | password | Sirius   | -lozenge |          |
|          |          | as       | Wallet   | .aui-    |          |
|          |          | before   |          | lozenge- |          |
|          |          | and      |          | success} |          |
|          |          | click on |          |          |          |
|          |          | "Sign    |          |          |          |
|          |          | in"      |          |          |          |
|          |          | button   |          |          |          |
+----------+----------+----------+----------+----------+----------+
| NEWWLT-9 | Address  | Checking | All      | [PAS     |          |
|          | book     | all      | a        | S]{.stat |          |
|          |          | a        | ddresses | us-macro |          |
|          |          | ddresses | in       | .aui     |          |
|          |          | of the   | address  | -lozenge |          |
|          |          | account  | book are | .aui-    |          |
|          |          | in old   | kept     | lozenge- |          |
|          |          | wallet   | intact   | success} |          |
|          |          | and new  | in old   |          |          |
|          |          | wallet   | wallet   |          |          |
|          |          |          | and new  |          |          |
|          |          |          | wallet   |          |          |
+----------+----------+----------+----------+----------+----------+
| N        | Private  | Checking | The      | [PAS     |          |
| EWWLT-10 | Key      | private  | private  | S]{.stat |          |
|          |          | key of   | key      | us-macro |          |
|          |          | the      | value of | .aui     |          |
|          |          | account  | the      | -lozenge |          |
|          |          | in old   | account  | .aui-    |          |
|          |          | wallet   | in the   | lozenge- |          |
|          |          | and new  | old      | success} |          |
|          |          | wallet   | wallet   |          |          |
|          |          |          | is the   |          |          |
|          |          |          | same as  |          |          |
|          |          |          | in the   |          |          |
|          |          |          | new      |          |          |
|          |          |          | wallet   |          |          |
+----------+----------+----------+----------+----------+----------+
| N        | Public   | Checking | The      | [PAS     |          |
| EWWLT-11 | Key      | public   | public   | S]{.stat |          |
|          |          | key of   | key      | us-macro |          |
|          |          | the      | value of | .aui     |          |
|          |          | account  | the      | -lozenge |          |
|          |          | in old   | account  | .aui-    |          |
|          |          | wallet   | in the   | lozenge- |          |
|          |          | and new  | old      | success} |          |
|          |          | wallet   | wallet   |          |          |
|          |          |          | is the   |          |          |
|          |          |          | same as  |          |          |
|          |          |          | in the   |          |          |
|          |          |          | new      |          |          |
|          |          |          | wallet   |          |          |
+----------+----------+----------+----------+----------+----------+
| N        | Wallet   | Checking | The      | [PAS     |          |
| EWWLT-12 | address  | wallet   | wallet   | S]{.stat |          |
|          |          | address  | address  | us-macro |          |
|          |          | of the   | value of | .aui     |          |
|          |          | account  | the      | -lozenge |          |
|          |          | in old   | account  | .aui-    |          |
|          |          | wallet   | in the   | lozenge- |          |
|          |          | and new  | old      | success} |          |
|          |          | wallet   | wallet   |          |          |
|          |          |          | is the   |          |          |
|          |          |          | same as  |          |          |
|          |          |          | in the   |          |          |
|          |          |          | new      |          |          |
|          |          |          | wallet   |          |          |
+----------+----------+----------+----------+----------+----------+
| N        | Multiple | Checking | All      | [PAS     |          |
| EWWLT-13 | accounts | multiple | accounts | S]{.stat |          |
|          |          | accounts | within a | us-macro |          |
|          |          | within a | wallet   | .aui     |          |
|          |          | wallet   | are kept | -lozenge |          |
|          |          | in old   | intact   | .aui-    |          |
|          |          | wallet   | in old   | lozenge- |          |
|          |          | and new  | wallet   | success} |          |
|          |          | wallet   | and new  |          |          |
|          |          |          | wallet   |          |          |
+----------+----------+----------+----------+----------+----------+
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
