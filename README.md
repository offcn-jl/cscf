# Chaos Go SCF ( Gin to SCF ) 
Chaos Go SCF ( Gin to SCF ) , A RESTFul WEB API Service Frame For SCF.

[![MIT license](https://img.shields.io/badge/license-MIT-brightgreen.svg)](https://opensource.org/licenses/MIT) [![Go Report Card](https://goreportcard.com/badge/github.com/offcn-jl/chaos-go-scf)](https://goreportcard.com/report/github.com/offcn-jl/chaos-go-scf) Master : ![Build](https://github.com/offcn-jl/chaos-go-scf/workflows/Build/badge.svg) New-Feature : ![Build](https://github.com/offcn-jl/chaos-go-scf/workflows/Build/badge.svg?branch=new-feature) 

基于 [Gin](https://github.com/gin-gonic/gin) 框架进行重写，舍弃 Router 组件 ( 使用 [API 网关](#APIGateway) 替代 ) 、多线程管理相关逻辑、各种加锁解锁逻辑，并对 [SCF](#SCF) 进行适配。预期实现对最终效果是可以直接将基于 Gin 框架编写的 Handler 迁移到 SCF 运行，实现将 Gin 的 Handler 作为 SCF "微服务" 运行的效果。

###### APIGateway
腾讯云 [API 网关](https://cloud.tencent.com/product/apigateway)（API Gateway）是[腾讯云](https://cloud.tencent.com)推出的一种 API 托管服务，能提供 API 的完整生命周期管理，包括创建、维护、发布、运行、下线等。
###### SCF
[云函数](https://cloud.tencent.com/document/product/583)（Serverless Cloud Function，SCF）是[腾讯云](https://cloud.tencent.com)为企业和开发者们提供的无服务器执行环境。
