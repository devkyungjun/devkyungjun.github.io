---
layout: post
title: "노마드코더 타입스크립트(1)"
description: 노마드코더 강의 타입스크립트의 학습 후기
date: 2022-05-08 20:00:07
hero_image: /assets/img/ts-lettermark-blue.png
hero_height: is-medium
hero_darken: true
image: /assets/img/ts-lettermark-blue.png
tags: 타입스크립트 Typescript
# canonical_url: https://www.csrhymes.com/2020/05/08/creating-a-docs-site-with-bulma-clean-theme.html
---

## 타입스크립트란?
TypeScript는 JavaScript에 추가적인 구문을 추가하여 editor와의 단단한 통합을 지원합니다. editor에서 초기에 오류를 잡을 수 있습니다.

TypeScript 코드는 JavaScript가 실행되는 모든 곳(브라우저, Node.js 또는 Deno 및 앱 등)에서 JavaScript로 변환될 수 있습니다.

TypeScript는 JavaScript를 이해하고 타입 추론(type inference)을 사용하여 추가 코드 없이도 훌륭한 도구를 제공합니다.

## 타입스트립트 타입 선언하기


타입스크립트에서 타입을 선언하는 기본 방법을 정리했습니다.
타입은 소문자, 대문자를 구별하므로 주의가 필요합니다.
TypeScript가 “기본 제공하는 타입”은 `모두 소문자입니다.` 

##### boolean
```bash
let isLoggedIn: boolean = false;
```
##### number
```bash
let age: number = 10;
```
##### string
```bash
let str: string = "hi";
let greeting: string = `Hello, my name is ${myName}.`; // ES6 템플릿 대입문
```
##### array
```bash
let arr: number[] = [1, 2, 3];

// 제네릭 배열 타입
let arr: Array<number> = [1, 2, 3];
```


## 타입스트립트 타입 추론
타입스크립트에서 위와같이 타입을 직접 선언할 수 있지만, javascript 처럼
:boolean -> type cheker 가 추론하는 방법이 있습니다.

##### 타입 추론
```bash
let a = "hi";
 => a 을 string 타입으로 추론
a = 1
 => string 타입에 number 타입 할당 불가 알림
```

## 타입스트립트 테스트 및 핸드북


[타입스크립트 코드 테스트](https://www.typescriptlang.org/play) 

[타입스크립트 핸드북](https://typescript-kr.github.io/pages/basic-types.html) 
