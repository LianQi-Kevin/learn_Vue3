# 配置Vue开发环境

## 1. 安装Nodejs

1. 访问 [Nodejs官网](https://nodejs.org)

2. 选择 LTS版（长期支持版）下载

   ![image-20230407103743223](https://cdn.jsdelivr.net/gh/LianQi-Kevin/Markdown_Image_Hosting/images/202304071037529.png)

3. 下载后的文件名称为：`node-vx.y.z-x64.msi``

   > `x.y.z`为当时的LTS版本号
   >
   > Win 平台为`.msi`文件，Linux 平台需要从源码编译安装

4. 运行下载的安装包进行安装，一直选`next`即可

   ![image-20230407104741505](https://cdn.jsdelivr.net/gh/LianQi-Kevin/Markdown_Image_Hosting/images/202304071047600.png)

5. 安装完成后打开 cmd 运行`npm -v`，即可判断是否安装成功

## 2. 配置npm镜像站

### 2.1 常用镜像站地址

| 站点         | 命令                                                         |
| ------------ | ------------------------------------------------------------ |
| 淘宝镜像站   | `npm config set registry https://registry.npmmirror.com`     |
| 腾讯镜像站   | `npm config set registry http://mirrors.cloud.tencent.com/npm/` |
| 华为云镜像站 | `npm config set registry https://mirrors.huaweicloud.com/repository/npm/` |

### 2.2 验证镜像设置

```shell
npm config get registry
```

> 如果返回配置的镜像站名称，则镜像站设置成功

