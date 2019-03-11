# <a name="how-to-run-the-completed-project"></a><span data-ttu-id="72637-101">如何运行已完成的项目</span><span class="sxs-lookup"><span data-stu-id="72637-101">How to run the completed project</span></span>

## <a name="prerequisites"></a><span data-ttu-id="72637-102">先决条件</span><span class="sxs-lookup"><span data-stu-id="72637-102">Prerequisites</span></span>

<span data-ttu-id="72637-103">若要在此文件夹中运行已完成的项目, 您需要以下各项:</span><span class="sxs-lookup"><span data-stu-id="72637-103">To run the completed project in this folder, you need the following:</span></span>

- <span data-ttu-id="72637-104">在开发计算机上安装了[node.js](https://nodejs.org) 。</span><span class="sxs-lookup"><span data-stu-id="72637-104">[Node.js](https://nodejs.org) installed on your development machine.</span></span> <span data-ttu-id="72637-105">如果您没有 node.js, 请访问上一个链接 "下载选项"。</span><span class="sxs-lookup"><span data-stu-id="72637-105">If you do not have Node.js, visit the previous link for download options.</span></span> <span data-ttu-id="72637-106">(**注意:** 本教程是使用节点版本10.7.0 编写的。</span><span class="sxs-lookup"><span data-stu-id="72637-106">(**Note:** This tutorial was written with Node version 10.7.0.</span></span> <span data-ttu-id="72637-107">本指南中的步骤可能适用于其他版本, 但尚未经过测试。</span><span class="sxs-lookup"><span data-stu-id="72637-107">The steps in this guide may work with other versions, but that has not been tested.)</span></span>
- <span data-ttu-id="72637-108">使用 Outlook.com 上的邮箱的个人 Microsoft 帐户, 或者是 microsoft 工作或学校帐户。</span><span class="sxs-lookup"><span data-stu-id="72637-108">Either a personal Microsoft account with a mailbox on Outlook.com, or a Microsoft work or school account.</span></span>

<span data-ttu-id="72637-109">如果你没有 Microsoft 帐户, 可以使用以下几种方法获取免费帐户:</span><span class="sxs-lookup"><span data-stu-id="72637-109">If you don't have a Microsoft account, there are a couple of options to get a free account:</span></span>

- <span data-ttu-id="72637-110">你可以[注册新的个人 Microsoft 帐户](https://signup.live.com/signup?wa=wsignin1.0&rpsnv=12&ct=1454618383&rver=6.4.6456.0&wp=MBI_SSL_SHARED&wreply=https://mail.live.com/default.aspx&id=64855&cbcxt=mai&bk=1454618383&uiflavor=web&uaid=b213a65b4fdc484382b6622b3ecaa547&mkt=E-US&lc=1033&lic=1)。</span><span class="sxs-lookup"><span data-stu-id="72637-110">You can [sign up for a new personal Microsoft account](https://signup.live.com/signup?wa=wsignin1.0&rpsnv=12&ct=1454618383&rver=6.4.6456.0&wp=MBI_SSL_SHARED&wreply=https://mail.live.com/default.aspx&id=64855&cbcxt=mai&bk=1454618383&uiflavor=web&uaid=b213a65b4fdc484382b6622b3ecaa547&mkt=E-US&lc=1033&lic=1).</span></span>
- <span data-ttu-id="72637-111">你可以[注册 office 365 开发人员计划](https://developer.microsoft.com/office/dev-program)以获取免费的 office 365 订阅。</span><span class="sxs-lookup"><span data-stu-id="72637-111">You can [sign up for the Office 365 Developer Program](https://developer.microsoft.com/office/dev-program) to get a free Office 365 subscription.</span></span>

## <a name="register-a-web-application-with-the-application-registration-portal"></a><span data-ttu-id="72637-112">在应用程序注册门户中注册 web 应用程序</span><span class="sxs-lookup"><span data-stu-id="72637-112">Register a web application with the Application Registration Portal</span></span>

1. <span data-ttu-id="72637-113">打开浏览器并导航到[应用程序注册门户](https://apps.dev.microsoft.com)。</span><span class="sxs-lookup"><span data-stu-id="72637-113">Open a browser and navigate to the [Application Registration Portal](https://apps.dev.microsoft.com).</span></span> <span data-ttu-id="72637-114">使用**个人帐户**(亦称: Microsoft 帐户) 或**工作或学校帐户**登录。</span><span class="sxs-lookup"><span data-stu-id="72637-114">Login using a **personal account** (aka: Microsoft Account) or **Work or School Account**.</span></span>

1. <span data-ttu-id="72637-115">选择页面顶部的 "**添加应用**"。</span><span class="sxs-lookup"><span data-stu-id="72637-115">Select **Add an app** at the top of the page.</span></span>

    > <span data-ttu-id="72637-116">**注意:** 如果在页面上看到多个 "**添加应用程序**" 按钮, 请选择与 "**聚合应用程序**" 列表对应的项。</span><span class="sxs-lookup"><span data-stu-id="72637-116">**Note:** If you see more than one **Add an app** button on the page, select the one that corresponds to the **Converged apps** list.</span></span>

1. <span data-ttu-id="72637-117">在 "**注册应用程序**" 页上, 将**应用程序名称**设置为**node.js Graph 教程**, 然后选择 "**创建**"。</span><span class="sxs-lookup"><span data-stu-id="72637-117">On the **Register your application** page, set the **Application Name** to **Node.js Graph Tutorial** and select **Create**.</span></span>

    ![在应用注册门户网站中创建新应用程序的屏幕截图](/tutorial/images/arp-create-app-01.png)

1. <span data-ttu-id="72637-119">在**node.js 图教程注册**页上的 "**属性**" 部分下, 复制**应用程序 Id** , 因为稍后将需要它。</span><span class="sxs-lookup"><span data-stu-id="72637-119">On the **Node.js Graph Tutorial Registration** page, under the **Properties** section, copy the **Application Id** as you will need it later.</span></span>

    ![新创建的应用程序 ID 的屏幕截图](/tutorial/images/arp-create-app-02.png)

1. <span data-ttu-id="72637-121">向下滚动到 "**应用程序机密**" 部分。</span><span class="sxs-lookup"><span data-stu-id="72637-121">Scroll down to the **Application Secrets** section.</span></span>

    1. <span data-ttu-id="72637-122">选择 "**生成新密码**"。</span><span class="sxs-lookup"><span data-stu-id="72637-122">Select **Generate New Password**.</span></span>
    1. <span data-ttu-id="72637-123">在 "**生成新密码**" 对话框中, 复制框中的内容, 因为稍后将需要它。</span><span class="sxs-lookup"><span data-stu-id="72637-123">In the **New password generated** dialog, copy the contents of the box as you will need it later.</span></span>

        > <span data-ttu-id="72637-124">**重要说明:** 此密码永远不会再次显示, 因此请务必立即复制它。</span><span class="sxs-lookup"><span data-stu-id="72637-124">**Important:** This password is never shown again, so make sure you copy it now.</span></span>

    ![新创建的应用程序密码的屏幕截图](/tutorial/images/arp-create-app-03.png)

1. <span data-ttu-id="72637-126">向下滚动到 "**平台**" 部分。</span><span class="sxs-lookup"><span data-stu-id="72637-126">Scroll down to the **Platforms** section.</span></span>

    1. <span data-ttu-id="72637-127">选择 "**添加平台**"。</span><span class="sxs-lookup"><span data-stu-id="72637-127">Select **Add Platform**.</span></span>
    1. <span data-ttu-id="72637-128">在 "**添加平台**" 对话框中, 选择 " **Web**"。</span><span class="sxs-lookup"><span data-stu-id="72637-128">In the **Add Platform** dialog, select **Web**.</span></span>

        ![为应用程序创建平台的屏幕截图](/tutorial/images/arp-create-app-04.png)

    1. <span data-ttu-id="72637-130">在 " **Web**平台" 框中, 输入`http://localhost:3000/auth/callback` **重定向 url**的 url。</span><span class="sxs-lookup"><span data-stu-id="72637-130">In the **Web** platform box, enter the URL `http://localhost:3000/auth/callback` for the **Redirect URLs**.</span></span>

        ![应用程序新添加的 Web 平台的屏幕截图](/tutorial/images/arp-create-app-05.png)

1. <span data-ttu-id="72637-132">滚动到页面底部, 然后选择 "**保存**"。</span><span class="sxs-lookup"><span data-stu-id="72637-132">Scroll to the bottom of the page and select **Save**.</span></span>

## <a name="configure-the-sample"></a><span data-ttu-id="72637-133">配置示例</span><span class="sxs-lookup"><span data-stu-id="72637-133">Configure the sample</span></span>

1. <span data-ttu-id="72637-134">将`.env.example`文件重命名`.env`为。</span><span class="sxs-lookup"><span data-stu-id="72637-134">Rename the `.env.example` file to `.env`.</span></span>
1. <span data-ttu-id="72637-135">编辑`.env`文件并进行以下更改。</span><span class="sxs-lookup"><span data-stu-id="72637-135">Edit the `.env` file and make the following changes.</span></span>
    1. <span data-ttu-id="72637-136">将`YOUR_APP_ID_HERE`替换为你从应用注册门户获取的**应用程序 Id** 。</span><span class="sxs-lookup"><span data-stu-id="72637-136">Replace `YOUR_APP_ID_HERE` with the **Application Id** you got from the App Registration Portal.</span></span>
    1. <span data-ttu-id="72637-137">将`YOUR_APP_PASSWORD_HERE`替换为你在应用注册门户中获取的密码。</span><span class="sxs-lookup"><span data-stu-id="72637-137">Replace `YOUR_APP_PASSWORD_HERE` with the password you got from the App Registration Portal.</span></span>
1. <span data-ttu-id="72637-138">在命令行界面 (CLI) 中, 导航到此目录并运行以下命令以安装要求。</span><span class="sxs-lookup"><span data-stu-id="72637-138">In your command-line interface (CLI), navigate to this directory and run the following command to install requirements.</span></span>

    ```Shell
    npm install
    ```

## <a name="run-the-sample"></a><span data-ttu-id="72637-139">运行示例</span><span class="sxs-lookup"><span data-stu-id="72637-139">Run the sample</span></span>

1. <span data-ttu-id="72637-140">在 CLI 中运行以下命令以启动应用程序。</span><span class="sxs-lookup"><span data-stu-id="72637-140">Run the following command in your CLI to start the application.</span></span>

    ```Shell
    npm start
    ```

1. <span data-ttu-id="72637-141">打开浏览器，然后转到 `http://localhost:3000`。</span><span class="sxs-lookup"><span data-stu-id="72637-141">Open a browser and browse to `http://localhost:3000`.</span></span>