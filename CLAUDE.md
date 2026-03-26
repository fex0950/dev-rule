# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is vlive-doc, a Chinese documentation repository for the vlive platform. It contains development guidelines, project documentation, and technical specifications for various components including video players and product selection centers.

## Repository Structure

- `/dev/` - Development guidelines and coding standards
- `/project/选品中心/` - Product selection center project documentation
- `/technical/player/` - Video player technical documentation
- `/doc/` - General documentation

## Language and Localization

- **Primary Language**: Chinese (zh-CN)
- All documentation should be written in Chinese
- Cursor is configured to use Chinese language (see `.cursorrules`)

## Coding Standards

Based on `/dev/lint.md`, follow these naming conventions:

- **枚举 (Enums)**: 大驼峰 with `Enum` suffix (e.g., `StatusEnum`)
- **函数 (Functions)**: 小驼峰
  - 回调函数: `handle` prefix (e.g., `handleClick`)
  - 事件发送: `on` prefix (e.g., `onSubmit`)
  - 动作函数: action prefix like `get`, `set` (e.g., `getUserData`)
- **变量 (Variables)**: 小驼峰 (camelCase)
- **常量 (Constants)**: 大写加下划线 (UPPER_SNAKE_CASE)
- **类 (Classes)**: 大驼峰 (PascalCase)
- **接口 (Interfaces)**: 大驼峰 with `I` prefix (e.g., `IUserData`)
- **类型 (Types)**: 大驼峰 (PascalCase)

## Project Domains

For the 选品中心 (Product Selection Center) project:

### 运营后台 (Admin Backend)
- Test: `adminjxlm-test.vlebo.cn`
- Production: `adminjxlm.vlebo.cn`

### 供应商端 (Supplier Portal)
- Test: `jxlm-test.vlebo.cn`
- Production: `jxlm.vlebo.cn`

## Technical Stack

- **Video Players**: TCPlayer 4.9.1 and 西瓜播放器 (XGPlayer)
- **Frontend Framework**: Vue 2 (based on `/dev/vue2.md`)
- **Language**: Chinese documentation and interface

## File Organization

When working with this repository:
- Place development guidelines in `/dev/`
- Project-specific documentation goes in `/project/[项目名]/`
- Technical specifications belong in `/technical/`
- Use descriptive Chinese filenames and maintain existing structure