# TeachOpenCADD

#### TeachOpenCADD: オープンソースのパッケージとデータを使ったコンピューター支援（CADD）ドラッグデザインの教育用プラットフォーム

Dominique Sydow, Andrea Morger, Maximilian Driller and Andrea Volkamer

*In Silico* Toxicology, Institute for Physiology, Universitätsmedizin Berlin, Virchowweg 6, 10117 Berlin

[![DOI](https://img.shields.io/badge/DOI-10.1186%2Fs13321--019--0351--x-blue.svg)](https://doi.org/10.1186/s13321-019-0351-x)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.2600909.svg)](https://doi.org/10.5281/zenodo.2600909)
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/volkamerlab/TeachOpenCADD/master)

質問がある場合は teachopencadd@charite.de に連絡してください。もしくは、このページにない講義用チュートリアルについての情報、チュートリアルのもととなるアイデアがあればぜひ連絡してください。

このページは　CC BY 4.0 ライセンスののもとで提供されています。ライセンスの詳細は　http://creativecommons.org/licenses/by/4.0/ をご覧ください。

## 目次  

* [この教育用プラットフォームの目的について](#この教育用プラットフォームの目的)
* [トピック](#トピック)
* [使い方](#使い方)

## この教育用プラットフォームの目的

([目次](#目次) に戻る)

コンピューター支援ドラッグデザイン (CADD)にとって、ケモインフォマティクスと構造バイオインフォマティクスに関するオープンソースのプログラミングパッケージは、パワフルなツールで、モジュール式かつ再現可能、簡単に共有可能なパイプラインを提供します。ところが、ツールの説明、ドキュメンテーションは利用可能な一方で、CADDの活用方法について焦点をあて、背景にあるコンセプトを教える上で、自由に利用可能な具体例はほんの少ししかありません。例を挙げれば TDT initiative と言ったものがあります。 [1]

ここでは、学生による学生のために開発されたCADDの教育用プラットフォームを提供します。使用するオープンソースパッケージはPythonツール、RDKit [2] 、PyPDB [3] 、そして PyMol [4] です。それぞれのトピックについて、インタラクティブなJupyter Notebook [5] を開発しました。Githubで自由に利用可能で、トピックに関する理論的な背景の詳細な説明と、詳しいコメント付きのPythonコードが書いてあります。EGFR キナーゼを例に、公共の化合物データベース ChEMBL [6] からデータを取得する方法、ドラッグライクネスの観点から化合物をフィルタリングする方法、好ましく無い部分構造をもつ化合物を探し出し取り除く方法を議論します。さらに、化合物の類似性を評価する方法を導入し、化合物のクラスター化を行い、多様性のある化合物セットをつくります。また、新規な活性化合物を予測するためのモデルを構築するため、機械学習のアプローチを導入します。最後に、公共のタンパク質データベース PDB [7] から構造を取得し、それらを使ってリガンドベースの3D ファーマコフォアの生成、オフターゲットを予測するために結合サイト比較を実施します。

このプラットフォームを作成したことの目的は、オープンソースのケモインフォマティクスツールに興味を持っている利用者に、いかに簡単に利用できて、どんな利点があるかということを紹介することです。取り上げるトピックは継続的に増やしていきますし、コミュニティからのコントリビューションもお待ちしています。教育目的の利用だけでなく、この Jupiter notebookは各プロジェクトに合わせて修正し拡張するための出発点としても使えます。

文献:

[1] [S. Riniker et al., F1000Research, 2017, 6, 1136](https://f1000research.com/articles/6-1136/v1)
[2] [G. Landrum, RDKit](http://www.rdkit.org)
[3] [W. Gilpin, Bioinformatics, 2016, 32, 156-60](https://academic.oup.com/bioinformatics/article/32/1/159/1743800)
[4] [The PyMOL Molecular Graphics System, Version 1.8, Schrödinger, LLC](https://pymol.org)
[5] [T. Kluyver et al., IOS Press, 2016, 87-90.](http://ebooks.iospress.com/publication/42900)
[6] [A. Gaulton et al., Nucleic Acid Res., 2017, 40, D1100-7](https://academic.oup.com/nar/article/42/D1/D1083/1043509)
[7] [H. Berman et al., Nucleic Acid Res., 2000, 28, 235-42](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC102472/)


## トピック

([目次](#目次) に戻る。)

TeachOpenCADDのトピックはいわゆる **トークトリアル（talkatorial）** の形式（理論とコードのミックスで、プレゼンテーション形式での発表にも利用可能な形式）で取り上げられていて、現在、以下の内容で構成されています：

ケモインフォマティクス :

* Topic 1. 化合物データの取得：ChEMBL
* Topic 2. 化合物フィルタリング：ADMEとリードライクネスのクライテリア
* Topic 3. 化合物フィルタリング：好ましく無い部分構造
* Topic 4. リガンドベーススクリーニング: 化合物類似性
* Topic 5. 化合物クラスタリング
* Topic 6. 最大共通部分構造（Maximum common substructures）
* Topic 7. リガンドベーススクリーニング：機械学習

構造バイオインフォマティクス：

* Topic 8. タンパク質データの取得：Protein Data Bank (PDB)
* Topic 9. リガンドベースファーマコフォア
* Topic 10. 結合サイトの類似性
* Topic 11. オンライン API/サーバー を使用した構造ベースのCADD
  * 11a. 潜在的なキナーゼ阻害剤を見つけるためのKLIFSとPubChemのクエリ化
  * 11b. 標的に対して候補のドッキングを行う
  * 11c. 結果の可視化と既知のデータとの比較

教育用の素材は次のフォーマットで提供されています：

* コーディングベースのJupyter Notebook（topics 1-11）はGithubのこのページにあり、いわゆるトークトリアル（talktorial = talk + tutorial）、つまりプレゼンテーションでも使えるチュートリアルの形式です。
* GUIベースのKNIME ワークフロー (topics 1-8) は [KNIME Hub](https://hub.knime.com/volkamerlab/space/TeachOpenCADD/TeachOpenCADD) で手に入ります。

## 使い方

([目次](#目次) に戻る。)

レポジトリと必要な依存関係にあるものを全てホストするためにBinderを使うことができます。あるいはローカルでトークトリアルを使うこともできます（レポジトリをダウンロートして、依存関係にあるものをインストールしてください）

### Binderの使い方 (対象トークトリアル T1-T8)

以下のリンクに従うことでレポジトリと必要な依存関係にあるものを全てホストするためにBinderを使うことができます:

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/volkamerlab/TeachOpenCADD/master)

セットアップには２、３分かかります。

### ローカル環境へのインストール (対象トークトリアル　全て)

#### Linux

1.  （トークトリアルを含む）TeachOpenCADDレポジトリのコピーをローカルに落としてください

    a. ... zipアーカイブとしてダウンロードしてunzipしてください：

    ![Download repository](https://github.com/volkamerlab/TeachOpenCADD/blob/master/README_figures/download_repo.png)

    b. ... もしくは `git` パッケージを使って自分のコンピュータにクローンしてください：

        ```bash
        git clone https://github.com/volkamerlab/TeachOpenCADD.git
        ```

2.  Anacondaソフトウェアを使ってパッケージのバージョン管理をクリーンにしてください。

    Anaconda2、あるいはAnaconda3をインストールします。理論上はインストールするAnacondaのバージョンの問題です。ですが、Anaconda2でしかテストしていないので、Anaconda3で同じような動作となるかは保証できません。

    https://docs.anaconda.com/anaconda/install/

3.  パッケージ管理システムcondaを使ってトーカトリアルの環境を作ります（ `teachopencadd` という名前をつけています）

    必要なパッケージをすべて含んでいる環境ファイル (yml file) を提供しています。

    ```bash
    conda env create -f environment.yml
    ```

    Note: この環境を手動でつくることもできます。
    ["別の方法：conda環境を手動で作る"](#別の方法：conda環境を手動で作る) を参照してください。

4.  作成したconda環境をアクティベートしてください。

    ```bash
    conda activate teachopencadd
    ```

    これでconda環境の中で作業することができます。

5.  作成したconda環境をJupyter notebook にリンクしてください

    ```bash
    python -m ipykernel install --user --name teachopencadd

    # FYI: このリンクをアンインストールするには以下のコマンドを使用してください:
    #jupyter kernelspec uninstall teachopencadd
    ```

6.  Jupyter notebookを起動してください。

    ```bash
    jupyter notebook
    ```

7.  メニューからJupyterのカーネルを作成したconda環境に変えてください。

    `Kernel > Change kernel > Python [conda env:teachopencadd]`

    ![Jupyterカーネルを変更する](https://github.com/volkamerlab/TeachOpenCADD/blob/master/README_figures/jupyter_kernel_teachopencadd.png)

8.  これで最初のトーカトリアル開始です。Enjoy!



##### 別の方法：conda環境を手動で作る

**Note**: これは上のステップ３で書かれているymlファイルを使用してconda環境をつくる方法の代わりとなる方法です。

```bash
# `teachopencadd` という名前の環境をつくりアクティベートします
conda create -n teachopencadd python=3.6
conda activate teachopencadd

# conda経由でパッケージをインストールします
conda install jupyter  # ipykernelもインストールします
conda install -c conda-forge rdkit  # umpy と pandas もインストールします
conda install -c samoturk pymol  # Linux: freeglut と glewもインストールします
conda install -c conda-forge pmw  # Pymolのターミナルウィンドウを立ち上げるのに必要です。
conda install -c conda-forge scikit-learn  # scipyをインストールします
conda install -c conda-forge seaborn  # matplotlibをインストールします
conda install -c conda-forge chembl_webresource_client
conda install -c conda-forge biopandas
conda install -c conda-forge pypdb
#conda install jupyter ipykernel pandas scikit-learn seaborn  # おそらくすでにインストールされていると思います。

# pip経由でパッケージをインストールします (おそらくデフォルトインストールされています）

pip install chembl_webresource_client biopandas pypdb
```

#### Windows

大枠では、LinuxとWindowsで同じように問題なくインストールできます。

唯一の違いはPyMolのインストール作業です。

* http://www.lfd.uci.edu/~gohlke/pythonlibs/#pymol　からPyMolをダウンロードします。
* Anaconda2 がインストールされている場所に置きます。(e.g. C:\Anaconda2)
* 管理者（administrator）コマンドプロンプトを開きます。 (Windows > accessories > command prompt, "右クリック" > 管理者として実行)
* プロンプトで正確なpathをタイプし、Anacondaのディレクトリに移動します。：

```bash
cd C:/Anaconda2
set path=%path%;C:\Anaconda2
pip install pymol‑2.3.0a0‑cp36‑cp36m‑win_amd64.whl
pip install pymol_launcher‑2.1‑cp36‑cp36m‑win_amd64.whl
# 上の文言はダウンロードした pymol_XXXX.whl ファイルに合わせてください
```

#### MacOS

Linux環境と同様にインストールできますが、```pymol``` をオープンソース ```samoturk``` condaチャンネルからインストールすることはできませんでした。代わりに```schrodinger``` チャンネルを使うことができます。残念ながらPyMOLを実行するにはSchrödingerライセンスが必要です（ライセンスは [教育目的](https://pymol.org/edu) の使用には無料で提供されています）。

インストールを手動で行うには、次のコマンドを：

```bash
conda install -c samoturk pymol # Installs also freeglut and glew
```

次に置き換えてください

```bash
conda install -c schrodinger pymol  # Installs also freeglut and glew
```

#### 出くわした問題

##### RDKit

* ```from rdkit.Chem.Draw import IPythonConsole``` がエラーメッセージ ```ImportError: No module named 'PIL'```を投げる:
`pip install pillow` のインストールを試してください(check out https://github.com/rdkit/rdkit/issues/1179)
* ```Draw.MolsToGridImage``` が Serial errorをだす: データのタイプを ```Draw.MolsToGridImage(list(df.ROMol), useSVG=True)``` のようにリストしてください。

##### pip

バージョン　10.0.X 以降のパッケージマネージャーは以前のものと動作が異なっています。上で使われているコマンドの```pip install chembl_webresource_client```は importエラー ```cannot import name main```を返します:

この問題はpython経由でpipを呼び出すことで解決することができます：

```bash
python3 -m pip install chembl_webresource_client
python3 -m pip install pypdb
```

```chembl_webresource_client``` をインストールする際に、 ```urllib3``` の互換性がないという警告が出るかもしれません。アップデートすることで解決することができます：

```bash
python3 -m pip install urllib3 --upgrade
```

解決方法は次からとりました。:

https://stackoverflow.com/questions/28210269/importerror-cannot-import-name-main-when-running-pip-version-command-in-window

## 連絡先

([目次](#目次) に戻る。)

質問や提案があれば連絡してください！

* Jupyter Notebookに関して質問があれば、GitHubレポジトリにイシューを立ててください: https://github.com/volkamerlab/teachopencadd/issues
* KNIMEワークフローについて質問があれば、KNIME Hubのページの「Discussion」セクションにポストを作成してください:  https://hub.knime.com/volkamerlab/space/TeachOpenCADD/TeachOpenCADD
* 新しいトピックについてアイデアがあれば、アンケートに記入してください: contribute.volkamerlab.org
* それ以外の全てのリクエストについてはe-mailを送ってください:  teachopencadd@charite.de

皆様からのご意見をお待ちしています！

## ライセンス

([目次](#目次) に戻る。)

この仕事は Attribution 4.0 International (CC BY 4.0) のもとでライセンスされています。このライセンスのコピーをみるには次のリンクを参照してください http://creativecommons.org/licenses/by/4.0/ 。

## 引用

([目次](#目次) に戻る。)

TeachOpenCADDプラットフォームの著者らは次の出資者からの公的出資を受け取っています:

* Bundesministerium für Bildung und Forschung (Grant Number 031A262C)
* Deutsche Forschungsgemeinschaft (Grant number VO 2353/1-1)
* HaVo-Stiftung, Ludwigshafen, Germany
* Stiftung Charité (Einstein BIH Visiting Fellow project)
* "SUPPORT für die Lehre" program (Förderung innovativer Lehrvorhaben) of the Freie Universität Berlin
* Open Access Publication Fund of Charité – Universitätsmedizin Berlin

サイエンティフィックな文献で TeachOpenCADD の教材を利用した時は、我々の文献を引用してください：

* [TeachOpenCADD Jupyter Notebooks: Talktorials 1-10.](https://jcheminf.biomedcentral.com/articles/10.1186/s13321-019-0351-x)
* [TeachOpenCADD KNIME workflows](https://pubs.acs.org/doi/full/10.1021/acs.jcim.9b00662)

TeachOpenCADDプラットフォームの有用さを計り、今後の出資をうけるために役立ちます！

@article{TeachOpenCADD2019,
    author = {Sydow, Dominique and Morger, Andrea and Driller, Maximilian and Volkamer, Andrea},
    doi = {10.1186/s13321-019-0351-x},
    journal = {J. Cheminform.},
    number = {1},
    pages = {29},
    title = {{TeachOpenCADD: a teaching platform for computer-aided drug design using open source packages and data}},
    url = {https://doi.org/10.1186/s13321-019-0351-x},
    volume = {11},
    year = {2019}
}

@article{TeachOpenCADDKNIME2019,
    author = {Sydow, Dominique and Wichmann, Michele and Rodr{\'{i}}guez-Guerra, Jaime and Goldmann, Daria and Landrum, Gregory and Volkamer, Andrea},
    doi = {10.1021/ACS.JCIM.9B00662},
    journal = {J. Chem. Inf. Model.},
    publisher = {American Chemical Society},
    title = {{TeachOpenCADD-KNIME: A Teaching Platform for Computer-Aided Drug Design Using KNIME Workflows}},
    url = {https://pubs.acs.org/doi/full/10.1021/acs.jcim.9b00662},
    year = {2019}
}
