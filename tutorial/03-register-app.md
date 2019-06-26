<!-- markdownlint-disable MD002 MD041 -->

<span data-ttu-id="84cd1-101">在本练习中, 你将使用 Azure Active Directory 管理中心创建新的 Azure AD web 应用程序注册。</span><span class="sxs-lookup"><span data-stu-id="84cd1-101">In this exercise, you will create a new Azure AD web application registration using the Azure Active Directory admin center.</span></span>

1. <span data-ttu-id="84cd1-102">打开浏览器，并转到 [Azure Active Directory 管理中心](https://aad.portal.azure.com)。</span><span class="sxs-lookup"><span data-stu-id="84cd1-102">Open a browser and navigate to the [Azure Active Directory admin center](https://aad.portal.azure.com).</span></span> <span data-ttu-id="84cd1-103">使用**个人帐户**（亦称为“Microsoft 帐户”）或**工作或学校帐户**登录。</span><span class="sxs-lookup"><span data-stu-id="84cd1-103">Login using a **personal account** (aka: Microsoft Account) or **Work or School Account**.</span></span>

1. <span data-ttu-id="84cd1-104">在左侧导航栏中选择 " **Azure Active Directory** ", 然后选择 "**管理**" 下的 "**应用程序注册**"。</span><span class="sxs-lookup"><span data-stu-id="84cd1-104">Select **Azure Active Directory** in the left-hand navigation, then select **App registrations** under **Manage**.</span></span>

    ![<span data-ttu-id="84cd1-105">应用注册的屏幕截图</span><span class="sxs-lookup"><span data-stu-id="84cd1-105">A screenshot of the App registrations</span></span> ](./images/aad-portal-app-registrations.png)

1. <span data-ttu-id="84cd1-106">选择“新注册”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="84cd1-106">Select **New registration**.</span></span> <span data-ttu-id="84cd1-107">在“注册应用”\*\*\*\* 页上，按如下方式设置值。</span><span class="sxs-lookup"><span data-stu-id="84cd1-107">On the **Register an application** page, set the values as follows.</span></span>

    - <span data-ttu-id="84cd1-108">将“名称”\*\*\*\* 设置为“`Node.js Graph Tutorial`”。</span><span class="sxs-lookup"><span data-stu-id="84cd1-108">Set **Name** to `Node.js Graph Tutorial`.</span></span>
    - <span data-ttu-id="84cd1-109">将“受支持的帐户类型”\*\*\*\* 设置为“任何组织目录中的帐户和个人 Microsoft 帐户”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="84cd1-109">Set **Supported account types** to **Accounts in any organizational directory and personal Microsoft accounts**.</span></span>
    - <span data-ttu-id="84cd1-110">在“重定向 URI”\*\*\*\* 下，将第一个下拉列表设置为“`Web`”，并将值设置为“`http://localhost:3000/auth/callback`”。</span><span class="sxs-lookup"><span data-stu-id="84cd1-110">Under **Redirect URI**, set the first drop-down to `Web` and set the value to `http://localhost:3000/auth/callback`.</span></span>

    !["注册应用程序" 页的屏幕截图](./images/aad-register-an-app.png)

1. <span data-ttu-id="84cd1-112">选择 "**注册**"。</span><span class="sxs-lookup"><span data-stu-id="84cd1-112">Select **Register**.</span></span> <span data-ttu-id="84cd1-113">在**Node.js Graph 教程**页上, 复制**应用程序 (客户端) ID**的值并保存它, 下一步将需要它。</span><span class="sxs-lookup"><span data-stu-id="84cd1-113">On the **Node.js Graph Tutorial** page, copy the value of the **Application (client) ID** and save it, you will need it in the next step.</span></span>

    ![新应用注册的应用程序 ID 的屏幕截图](./images/aad-application-id.png)

1. <span data-ttu-id="84cd1-115">选择“管理”\*\*\*\* 下的“身份验证”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="84cd1-115">Select **Authentication** under **Manage**.</span></span> <span data-ttu-id="84cd1-116">找到“隐式授予”\*\*\*\* 部分，并启用“ID 令牌”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="84cd1-116">Locate the **Implicit grant** section and enable **ID tokens**.</span></span> <span data-ttu-id="84cd1-117">选择“保存”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="84cd1-117">Select **Save**.</span></span>

    ![隐式 grant 部分的屏幕截图](./images/aad-implicit-grant.png)

1. <span data-ttu-id="84cd1-119">选择“管理”\*\*\*\* 下的“证书和密码”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="84cd1-119">Select **Certificates & secrets** under **Manage**.</span></span> <span data-ttu-id="84cd1-120">选择“新客户端密码”\*\*\*\* 按钮。</span><span class="sxs-lookup"><span data-stu-id="84cd1-120">Select the **New client secret** button.</span></span> <span data-ttu-id="84cd1-121">在 "**说明**" 中输入一个值, 然后选择 "**过期**" 选项之一, 然后选择 "**添加**"。</span><span class="sxs-lookup"><span data-stu-id="84cd1-121">Enter a value in **Description** and select one of the options for **Expires** and select **Add**.</span></span>

    !["添加客户端密码" 对话框的屏幕截图](./images/aad-new-client-secret.png)

1. <span data-ttu-id="84cd1-123">离开此页前，先复制客户端密码值。</span><span class="sxs-lookup"><span data-stu-id="84cd1-123">Copy the client secret value before you leave this page.</span></span> <span data-ttu-id="84cd1-124">将在下一步中用到它。</span><span class="sxs-lookup"><span data-stu-id="84cd1-124">You will need it in the next step.</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="84cd1-125">此客户端密码不会再次显示，所以请务必现在就复制它。</span><span class="sxs-lookup"><span data-stu-id="84cd1-125">This client secret is never shown again, so make sure you copy it now.</span></span>

    ![新添加的客户端密码的屏幕截图](./images/aad-copy-client-secret.png)