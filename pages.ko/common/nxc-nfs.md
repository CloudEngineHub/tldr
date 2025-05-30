# nxc nfs

> NFS 서버에 대한 펜테스트 및 익스플로잇 도구. 현재는 익명 모드만 지원.
> 더 많은 정보: <https://www.netexec.wiki/nfs-protocol>.

- 원격 NFS 서버의 버전 감지:

`nxc nfs {{192.168.178.0/24}}`

- 사용 가능한 NFS 공유 목록 나열:

`nxc nfs {{192.168.178.2}} --shares`

- 노출된 공유를 지정된 깊이까지 재귀적으로 열거:

`nxc nfs {{192.168.178.2}} --enum-shares {{5}}`

- 지정된 원격 파일 다운로드:

`nxc nfs {{192.168.178.2}} --get-file {{경로/대상/원격_파일}} {{경로/대상/로컬_파일}}`

- 지정된 로컬 파일을 원격 공유에 업로드:

`nxc nfs {{192.168.178.2}} --put-file {{경로/대상/로컬_파일}} {{경로/대상/원격_파일}}`
