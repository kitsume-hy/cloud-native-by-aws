
Elastic Container Service とは、Dockerを塚ttあ計算機クラスターをAWS宇えに作成するためのツールである。
ECSを使用することで、Dockerにパッケージされたアプリケーションを計算機クラスターに投入したり、起算気クラスターのインスタンスを追加。削除する操作を行うことができる.

ECSのがいようをしめしたのおが、ECSはタスクとよばれる単位で管理された計算ジョブを受け付ける。
システムにタスクが投入されっると、ECSは最初にタスクで指定されたDockerime-ji wo外部レジストリからダウンロードしてくる。
　AWS独自のDockerレジストリであるECR(Elaastic Container Registry)を指定することができる。

ECSの次の重要な役割はタスクの配置である。
あらかじめ定義されたクラスター内で、計算負荷がちいさい仮想インスタンスを選び出す。といったが、具体的にどのような戦略・ポリシーでこの選択を行うかは、ユーザーの指定したパラメータに従う。

また、クラスターのスケーリングもECSにおける重要な概念だる。スケーリングとは、クラスター内のインスタンスの計算負荷をモニタリングし、計算負荷に応じて