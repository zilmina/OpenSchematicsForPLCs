# OpenSchematicsForPLCs

## プロジェクト概要 / Project Overview

OpenSchematicsForPLCsは、様々なPLCシステムの包括的かつ詳細な回路図を提供することを目指しています。ユーザーが高品質で正確なオープンソースの回路設計にアクセスできるようにします。このライブラリには、複数のメーカーのデザインが含まれており、単一のリポジトリに統一することでアクセスとコラボレーションを簡素化しています。このプロジェクトは、教育および業務ニーズの両方をサポートすることを目的としています。

The OpenSchematicsForPLCs aims to provide comprehensive and detailed schematic diagrams for various PLC systems, ensuring that users have access to high-quality, accurate, and open-source circuit designs. This library includes designs from multiple manufacturers, unified under a single repository to streamline access and collaboration. This project is designed to support both educational and professional needs in the FA industry.

実験用電源遮断装置のリポジトリはOpenSchematicsForPLCsのサンプルであり、OpenSchematicsForPLCsをサブリポジトリとして利用しています。

The repository for the experimental power shutdown device serves as a sample for OpenSchematicsForPLCs. The experimental power shutdown device repository utilizes OpenSchematicsForPLCs as a subrepository.

## ライブラリに記載されている機材 / Equipment Listed in the Library

- **Beckhoff EL1889**: Digital Input Terminal
- **Beckhoff EL2889**: Digital Output Terminal
- **Beckhoff EL4002**: Analog Output Terminal
- **Beckhoff EL5101**: Incremental Encoder Interface
- **Beckhoff EK1828**: EtherCAT Coupler
- **Mitsubishi MR-J4-10A1**: Servo Amplifier
- **PILZ PNOZ e1vp**: Safety Controller

## インストール方法 / Installation

1. **リポジトリをクローンする / Clone the Repository**:
    ```bash
    git clone https://github.com/zilmina/OpenSchematicsForPLCs.git
    cd OpenSchematicsForPLCs
    ```

2. **KiCadのインストール / Install KiCad**:
    - 公式ウェブサイトからKiCadをダウンロードしてインストールします: [KiCad EDA](https://kicad.org/)

## サンプルを探す / Explore Examples
下記のリポジトリを参照してください。サンプル回路図やコードが記載されています。
- [実験用電源遮断装置 / SafetyPowerSupply](https://github.com/zilmina/ExperimentalPowerShutdownDevice)

## 貢献方法 / Contributing
コントリビューターは、製品のデータシートに記載されたリファレンスデザインに従い、KiCadを使用してリッチでコンポーネントに正確な回路図を作成することが推奨されています。
コミュニティからの貢献を歓迎します。高い一貫性と品質を確保するため、以下のガイドラインに従ってください。

Contributors are encouraged to adhere to reference designs provided in product datasheets and to create rich, component-accurate schematics using KiCad.
We welcome contributions from the community. To ensure consistency and high quality, please follow these guidelines:

1. **リファレンスデザインに従う / Adhere to Reference Designs**:
    - すべての回路図は、製品のデータシートに記載されたリファレンスデザインに従う必要があります。
    - All schematics must follow the reference designs provided in the product datasheets.

2. **詳細な回路図を作成する / Create Detailed Schematics**:
    - KiCadを使用して、コンポーネントの形状と配置を正確に反映したリッチな回路図を作成します。
    - Use KiCad to create rich, component-accurate schematics that reflect the true shapes and configurations of components.

3. **ファイル形式 / File Formats**:
    - 必要なGerberファイル、BOM（部品表）、CPL（部品配置リスト）を含めます。
    - Include necessary Gerber files, BOM (Bill of Materials), and CPL (Component Placement List).

4. **部品点数の削減に注力する / Focus on Component Reduction**:
    - JLCPCB向けの設計では、ノイズリダクションよりも部品点数の削減に注力してください。
    - Prioritize reducing the number of components over noise reduction when designing for JLCPCB.

5. **PCBA対応 / PCBA Compatibility**:
    - 可能な限りPCBA（プリント基板アセンブリ）に対応し、OSSユーザーがハンダ付けを最小限に抑えられるように設計してください。
    - Ensure designs are as ready for PCBA (Printed Circuit Board Assembly) as possible to minimize the need for soldering by OSS users.

6. **コントリビューターの認知 / Contributor Recognition**:
    - コントリビューターの名前やログをテスト基板に含めることが推奨されます。以下の推奨設定を使用してください。
    - Contributors are encouraged to include their names and logs on the test boards. Please use the recommended settings:
      - 印刷可能な面積 / Printable area: 右下角に2cm² / 2 cm² in the lower-right corner.
      - フォントサイズ / Font size: 読みやすさのために最小1.5mm / Minimum of 1.5 mm for readability.

## JLCPCBガイドライン / JLCPCB Guidelines

手軽で低コストなPCB製造を促進するため、以下のガイドラインに従ってください。

To facilitate easy and cost-effective PCB manufacturing, follow these guidelines for JLCPCB orders:

1. **推奨される部品の選定 / Recommended Components**:
    - コストパフォーマンスに優れた部品を選定すること。
    - Select cost-effective and readily available components.

2. **発注手順 / Ordering Steps**:
    1. JLCPCBのアカウントを作成する / Create a JLCPCB account.
    2. 必要なファイルをアップロードする（Gerber、BOM、CPL） / Upload the necessary files (Gerber, BOM, CPL).
    3. 設定を確認する（基板サイズ、層数、仕上げ） / Confirm settings (board size, layers, finish).
    4. 見積もりを確認する / Review the quote to ensure low cost.
    5. 発注を完了する / Complete the order.

3. **ファイル例 / File Examples**:
    - PCB設計のためのGerberファイル / Gerber files for PCB design.
    - 部品リストのBOM / BOM for the list of components.
    - 部品配置情報のCPL / CPL for component placement.

## コントリビューターのメリット / Benefits for Contributors

- **コミュニティの信頼と認知度 / Community Trust and Recognition**: Gain trust and recognition within the open-source community.
- **プロフェッショナルなスキルの向上 / Professional Skill Enhancement**: Improve your circuit design and KiCad skills through real-world projects.
- **スターやフォークの獲得 / Star and Fork Achievements**: See your work appreciated by many through stars and forks.
- **ネットワーキング / Networking Opportunities**: Connect with other engineers and developers.
- **学習と成長 / Learning and Growth**: Stay updated with new technologies and best practices.
- **求職者のためのメリット / Visibility for Job Seekers**: Contributors seeking employment can have their email addresses and corresponding folders listed in the README.md for professional visibility.

## お問い合わせ / Contact

ご質問がある場合は、リポジトリのメンテナにご連絡ください。

For any questions, please reach out to the repository maintainers.

---

OpenSchematicsForPLCsを、FA業界の皆様にとって貴重なリソースとするため、皆様の貢献と協力をお待ちしております。

We look forward to your contributions!
