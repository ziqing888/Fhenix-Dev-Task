#Fhenix 开发任务指南
<h2 align="center">Fhenix 开发任务</h2>
加入 Discord
创建 Discord 账户： 如果您还没有账户，请先 注册 Discord。
加入服务器： 点击 Fhenix Discord 加入服务器。
访问机器人命令：
导航到 #🤖|bot-commands 频道。
输入 /quests，然后从下拉菜单中选择 /quests 选项。
按 Enter 键查看可用任务。
图1：在 Discord 中访问机器人命令

网络设置
访问 Chainlist： 前往 Chainlist。
连接钱包：
点击 Connect wallet。
在您喜欢的钱包（如 Metamask、Rabby 或 OKX）中添加 Fhenix Helium 网络：
Metamask
Rabby
OKX Wallet
水龙头 (桥接)
获取 tFHE 代币：
挖矿： 通过 这里 挖矿获取 tFHE。
桥接： 使用以下网站从其他测试网桥接代币：
Native Bridge（Sepolia Ethereum → Fhenix Helium）
Pheasant Bridge（支持多个测试网络）
任务 4：在 Fhenix 上部署合约
访问 Remix 网站： 前往 Remix 网站。

图2：Remix IDE 界面

创建 Solidity 文件：

给文件命名，确保以 .sol 结尾（例如 zun.sol），然后按 Enter 键。
粘贴合约代码：

将以下 Solidity 代码复制并粘贴到新创建的文件中：
solidity
复制代码
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.26;

contract SimpleStorage {
    uint256 public storedData;

    function set(uint256 x) public {
        storedData = x;
    }

    function get() public view returns (uint256) {
        return storedData;
    }
}
编译合约：

点击左侧栏中的 Solidity Compiler 图标。

图4：Solidity 编译器

点击 Compile YOUR_CONTRACT_NAME.sol 按钮。

图5：编译合约

部署合约：

点击左侧栏中的 Deploy and run transactions 图标。

图5：部署与运行交易

打开您的钱包，并切换到 Fhenix Helium 网络（如果尚未切换）。

在环境设置中选择 Injected Provider，然后选择您的钱包。

点击 Deploy 按钮部署合约。

图6：部署合约按钮

确认部署：

恭喜，您已成功在 Fhenix Helium 上部署合约。

您可以在此处查看您的部署合约地址：

图7：查看合约地址

部署限制：

目前，您最多可以部署 5 个合约并获得 150 积分。
要部署更多合约，请重复点击 Deploy 按钮。
重复此过程 4 次以部署 4 个合约。
任务 6：合约验证
自动验证：

如果您使用上述合约代码，它将自动通过验证，您无需进行任何操作。

图：自动验证状态
`
