# 基于`logviewer` 的二次修改

该库主要服务于 `https://github.com/AlianBlank/GameFrameX` 作为子库使用。

# 使用方式(三种方式)

1. 直接在 `manifest.json` 文件中添加以下内容
   ```json
      {"com.sharelib.logviewer": "https://github.com/AlianBlank/com.sharelib.logviewer.git"}
    ```
2. 在Unity 的`Packages Manager` 中使用`Git URL` 的方式添加库,地址为：https://github.com/AlianBlank/com.sharelib.logviewer.git

3. 直接下载仓库放置到Unity 项目的`Packages` 目录下。会自动加载识别

# 改动功能

1. 删除每次编译都生成build_info 文件
2. 增加 `link.xml` 防止代码裁剪
[package.json](package.json)
----------------------------------------------------------------------------------------------------------

# Unity-Logs-Viewer[package.json](package.json)

Please note with new unity you can view device logs on editor console window, check the new attach menu in editor console window.

Using this tool you can easily check your editor console logs inside the game itself!
All what you have to do is to make a circle gesture using your mouse (click and drag) or your finger (touch and drag) on the mobile screen to show all these logs!

You can download also from unity asset store
https://www.assetstore.unity3d.com/en/#!/content/12047

#### To setup log viewer do the following

    1 - create reporter from menu (Reporter->Create) at first scene your game start.
    2 - then set the ” Scrip execution order ” in (Edit -> Project Settings ) of Reporter.cs to be the highest.

### Version 1.8

    - Add Copy to clipboard.
	- Merge Fix for Unity 2019.
	- Fix ReporterModificationProcessor is annoying.
	- Fix waste ram.

### Version 1.7

    - Add Save logs button( thanks for Ahmed Shbli ).
    - Fix deprecated code for new unity.
    - Fix Warnings.
    - Fix loading scene from asset bundle error.

<a href="https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J9MX5C6Q7B2NY">
    <img src="https://www.paypalobjects.com/webstatic/en_US/btn/btn_donate_cc_147x47.png">
    </img>
</a>
