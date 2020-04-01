# 个人简介
我是柯柯，一个机械狗 => 前端 => 后端。
学过且使用的语言有以下几种：
. JavaScript
. Python
. PHP
. Java

喜欢：
- 看电影
- 刷知乎
- 玩游戏

js代码示例：
`let a = 1`

Java代码示例：
```
package com.github.hcsp.shell;

import java.io.File;
import java.nio.file.Path;
import java.nio.file.Paths;
import java.util.Map;

public class Fork {

    public static void main(String[] args) throws Exception {
        ProcessBuilder pb = new ProcessBuilder("sh", "run.sh");
        Map<String, String> env = pb.environment();
        env.put("AAA", "123");
        pb.directory(getWorkingDir());
        pb.redirectOutput(getOutputFile());
        pb.start().waitFor();
    }

    private static File getWorkingDir() {
        Path projectDir = Paths.get(System.getProperty("user.dir"));
        return projectDir.resolve("working-directory").toFile();
    }

    private static File getOutputFile() {
        return new File(getWorkingDir(), "output.txt");
    }
}

```
