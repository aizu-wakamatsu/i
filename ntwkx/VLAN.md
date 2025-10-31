[参考リンク](https://milestone-of-se.nesuke.com/nw-basic/ethernet/vlan/)

# 基本知識


# 機能

L2SWとホストの間はポートベースでVLAN IDを設定する
VLANによってブロードキャストドメインが分割できる
	ほかのVLANのARPパケットは受信できない
同じセグメントのIPアドレスでもVLAN IDが違うと通信できない

# VLAN ID
1~4094のVLAN IDが利用可能

# タグVLAN

L2SWとL3SWの間で複数のVLANを1本のケーブルに束ねて伝送するのに使われる