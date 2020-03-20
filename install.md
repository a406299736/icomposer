1.  准备
	GitHub账号 https://www.github.com
	Packagist账号 https://packagist.org/

2. 可先在github上创建一个空仓库，然后克隆到本地，接下来创建自己的项目icomp。在icomp下新建一个composer.json文件，用来描述项目信息，提交到Packagist会检测这个文件，
	文件内容大致如下：
	{
    "name": "your-vendor-name/package-name",
    "description": "A short description of what your package does",
    "type": "project",
    "license": "MIT",
    "minimum-stability": "stable",
    "require": {}
	}
	详细见：https://packagist.org/about
	配置详情见：http://docs.phpcomposer.com/04-schema.html
	最后可以用 composer validate 命令验证一下。
	修改完后提交到 GitHub 版本库。

3. 在 Packagist 官网提交你的 Package。
	进入 Packagist 官网，登录你的账户，点击 Submit。
	填写你提交到 GitHub 的仓库地址。点击 Check，根据提示提交即可。
	稍等片刻，你会看到如下界面，然后你就可以使用这个库了。
	到这里就结束了吗？NO NO NO，如果你修改代码，它还不能自动更新。

4. Packagist 包自动更新
	Go to your GitHub repository
	Click the "Settings" button
	Click "Integrations & services"
	Add a "Packagist" service, and configure it with your API token, plus your Packagist username
	Check the "Active" box and submit the form

	详细见：https://packagist.org/about
	管理包版本库详见：https://packagist.org/about
