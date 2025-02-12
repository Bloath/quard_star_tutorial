[![CI](https://github.com/QQxiaoming/quard_star_tutorial/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/QQxiaoming/quard_star_tutorial/actions/workflows/ci.yml)
[![Documentation Status](https://readthedocs.org/projects/quard-star-tutorial/badge/?version=latest)](https://quard-star-tutorial.readthedocs.io/zh_CN/latest/?badge=latest)
[![CodeFactor](https://www.codefactor.io/repository/github/qqxiaoming/quard_star_tutorial/badge)](https://www.codefactor.io/repository/github/qqxiaoming/quard_star_tutorial)
[![GitHub All Releases](https://img.shields.io/github/downloads/QQxiaoming/quard_star_tutorial/total.svg)](https://github.com/QQxiaoming/quard_star_tutorial/releases)
[![GitHub stars](https://img.shields.io/github/stars/QQxiaoming/quard_star_tutorial.svg)](https://github.com/QQxiaoming/quard_star_tutorial)

# 基于qemu从0开始构建嵌入式linux系统

[English](./README.md) | 简体中文

![logo](./doc/img/img6.gif)

## 引言

本项目旨在真正从0开始构建嵌入式linux系统，为了剖析芯片从上电开始执行第一条指令到整个系统运行，相关应用服务启动，因此不使用市面上真实的板子，基于qemu定制模拟器开发板，且不使用qemu提供的快速加载elf的文件方式，因而我们需要下载qemu-6.0.0源码，自己编写(或使用qemu自带的)硬件ip相关模拟代码定制属于自己的硬件板卡。本项目同步制作[博客专栏](https://blog.csdn.net/weixin_39871788/category_11180842.html)(2021.8.11:目前开始使用readthedocs构建[文档](https://quard-star-tutorial.readthedocs.io/zh_CN/latest/index.html)，与博客内容相同)，因此项目尽量保证每增加一个feature就提交一次，方便索引跟踪开发过程以方便对应到博客的具体章节。

## 环境搭建

ubuntu18.04需要使用apt安装的包:

```shell
sudo apt install ninja-build pkg-config libglib2.0-dev libpixman-1-dev libgtk-3-dev libcap-ng-dev libattr1-dev device-tree-compiler bison flex
```

## 硬件架构

下图为目前的虚拟硬件架构，随着项目推进会持续更新。

![硬件架构](./doc/img/img3.png)

## 软件流程

下图为目前的软件流程，随着项目推进会持续更新。

![软件流程](./doc/img/img4.png)

## 内存分布

下图为目前的内存分布，随着项目推进会持续更新。

![内存分布](./doc/img/img5.png)

## 开发记录

[开发日记](./DEVELOPNOTE.md)
