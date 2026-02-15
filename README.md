# Molecular-Model-Maker
🧪 結晶構造 3D Generator / Crystal Structure 3D Generator
高校化学の学習を支援する、結晶格子の可視化・3Dモデル生成ツールです。
This is a web-based 3D visualization tool designed to help students understand crystal lattice structures in high school chemistry.
🌟 概要 / Overview「
教科書の2D図面だけでは理解しにくい、結晶内部の原子のつながりやパッキング」を解決するために開発しました。特に体心立方格子（BCC）を $(110)$ 面（1:√3面）で切断した状態を3Dで再現することに特化しており、生成したモデルはOBJ形式で書き出し可能です。
This tool solves the challenge of visualizing atomic connections within a crystal, which is often difficult to grasp from 2D textbook diagrams. It specifically features the ability to slice a Body-Centered Cubic (BCC) lattice along the $(110)$ plane.
🚀 主な機能 / Key Features
倍率選択 (Scaling): 1億倍〜5億倍の実寸スケーリング設定。精密カット (Precision Slicing): BCCの $(110)$ 面による斜め分割表示機能。3D出力 (3D Export): 3Dプリンタや他の3Dソフトで利用可能なOBJ形式でのエクスポート。断面図表示 (Section View): 幾何学的な原子の接触関係（対角線上のパッキング）を2Dでプレビュー。
🛠 使用技術 / Tech StackLanguage: Python 3.xUI Framework: Streamlit3D Geometry: Trimesh / NumPyVisualization: Matplotlib
💡 開発のこだわり / Technical Highlights単なる表面的な3D表示ではなく、3Dメッシュの切断アルゴリズム（Boolean演算）を実装しました。結晶幾何学に基づき、原子の中心座標と半径から数学的に正しい切断面（断面の比率 $1:\sqrt{2}$ および接線 $\sqrt{3}a$）を動的に生成することに注力しました。Beyond simple 3D rendering, 
I implemented a 3D mesh slicing algorithm using Boolean operations. This allows the tool to dynamically generate mathematically accurate cross-sections based on crystallographic geometry (e.g., the $1:\sqrt{2}$ aspect ratio and $\sqrt{3}a$ atomic contact lines).
