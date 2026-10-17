# Elephant DICOM Viewer（小象阅片器）

**中文** | [English](#english)

一款免费的 Windows 轻量 DICOM 阅片软件，面向**教学与科研展示**。免安装，下载后双击即可运行；所有数据只在你的电脑上处理，**不联网、不上传**。

> **重要声明**：本软件仅用于教学和科研展示，**不是医疗器械，不能用于诊断**，也不能作为临床决策的依据。使用时请勿处理未经授权的病人数据。

## 下载

到 [Releases（发行版）](../../releases/latest) 页面下载最新的 zip 压缩包，解压后双击 `ElephantDicomViewer.exe`。

- 系统：Windows 10（1607 及以上）或 Windows 11，64 位
- 无需安装，无需另装 .NET；文件约百余 MB（内含运行库）
- 程序未做数字签名，Windows 可能提示"未知发布者"：点"更多信息 → 仍要运行"即可
- 详细用法见压缩包里的 `README_CN.docx`

## 主要功能

- 打开 DICOM 文件夹 / ZIP / NIfTI / 普通图片；支持压缩 DICOM（JPEG、JPEG 2000、JPEG-LS）、多帧 DICOM、4D NIfTI
- 多窗格对比与联动、平铺（Tile）、三平面重建（MPR，可倾斜）
- 3D 视图：MIP / MinIP / 平均 / 容积渲染 / 面渲染；可用勾画工具切除或保留局部
- 测量：距离、角度、ROI（面积、均值、SD、最大/最小）、点值，可跨层、跨平面
- PET：SUV（体重法）读数与窗位预设；两个序列的融合（如 PET 叠加 CT）
- 病灶体积（出血、肿瘤）：勾画 + 插值 + 三维区域生长，输出体积与掩模
- 导出：图片、DICOM 拷贝（匿名化可选）、NIfTI、处理后的 3D 结果

## 反馈与问题

请在本页上方的 **Issues** 里提问或反馈。为便于定位，请尽量附上：操作步骤、序列类型（MR / CT / PET，厂家）、截图、报错弹窗文字。

> **请勿**在 Issues 或截图里放出病人姓名、ID、出生日期等隐私信息。

这是个人项目，欢迎反馈，但不保证及时回复。

## 许可与致谢

- 使用条款见 [TERMS.md](TERMS.md)；第三方组件声明见 `THIRD_PARTY_NOTICES.txt`（包含在下载的压缩包里）。
- 作者：Dr. WJ Zhou and Claude
- 使用了 [fo-dicom](https://github.com/fo-dicom/fo-dicom) 及其编解码库，感谢这些开源项目。
- 本软件的使用习惯参考了常见的 DICOM 阅片软件，但与任何商业产品无关联。

---

## English

**Elephant DICOM Viewer** is a free, lightweight DICOM viewer for Windows, intended for **teaching and research demonstration only**. No installation is needed; everything runs locally and **nothing is uploaded**.

> **Disclaimer**: This software is **not a medical device and must not be used for diagnosis** or any clinical decision. Do not process patient data you are not authorized to use.

**Download**: get the latest zip from the [Releases](../../releases/latest) page, unzip it and run `ElephantDicomViewer.exe`. Windows 10 (1607+) / 11, 64-bit. The program is not code-signed, so SmartScreen may show "unknown publisher" (More info → Run anyway). The user guide (`README_CN.docx`) is in Chinese.

**Features**: DICOM (including compressed and multi-frame), NIfTI and ordinary images; multi-pane linking, tile mode, MPR; 3D views (MIP, MinIP, average, volume and surface rendering) with a cut tool; measurements and ROI statistics; PET SUV (body weight) and fusion of two series; lesion volume tool; export to images, DICOM (optional anonymization), NIfTI, and processed 3D results.

**Feedback**: please open an **Issue** with steps to reproduce, modality / vendor and a screenshot. Never post patient-identifying information. This is a personal project; replies are not guaranteed.

**Credits**: Dr. WJ Zhou and Claude. Built on [fo-dicom](https://github.com/fo-dicom/fo-dicom) and its codecs; see `THIRD_PARTY_NOTICES.txt` in the download.
