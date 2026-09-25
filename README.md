# video-frame-notes

A Codex skill that processes video links or local videos, extracts and checks video frames, and creates timestamped Chinese notes from the visuals, audio, and subtitles. The notes include additional explanations to make key ideas easier to understand. When processing is complete, only the notes are kept; generated videos, frames, and other temporary files are deleted.

## Installation

Place this repository in your Codex skills directory so that the file is located at:

`~/.codex/skills/video-frame-notes/SKILL.md`

Start a new Codex session and invoke it with `$video-frame-notes`.

## Requirements

- Codex
- Node.js 22 or later to run `web-access`
- The `web-access` skill, installed separately for processing video links
- FFmpeg, preferably with `ffprobe`, for video decoding and frame extraction
- Chrome or Edge for websites that require browser access or login
- Chinese OCR and speech transcription tools when the video contains on-screen text or has no subtitles

This repository contains the skill instructions only. It does not include the tools listed above, browser credentials, or speech recognition models.


# video-frame-notes

一个 Codex skill：处理视频链接或本地视频，逐帧核对画面，并结合声音、字幕生成带时间戳和补充讲解的中文笔记。完成后只保留笔记，清理本次生成的视频、帧和其他临时文件。

## 安装

将本仓库放到 Codex 的 skills 目录，确保路径为：

`~/.codex/skills/video-frame-notes/SKILL.md`

然后重新打开 Codex 会话，使用 `$video-frame-notes` 调用。

## 所需工具

- Codex
- Node.js 22+：运行 web-access
- web-access skill：处理视频链接时需要单独安装
- FFmpeg，建议同时安装 ffprobe：视频解码与逐帧处理
- Chrome 或 Edge：部分网站需要浏览器访问或登录
- 中文 OCR、语音转写工具：视频有课件文字或没有字幕时需要相应能力

本仓库只提供 skill 规则，不包含上述工具、浏览器登录信息或语音模型。