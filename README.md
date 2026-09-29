# 暴力漂移赛车 (Drift Race)

## 老大需求(09-29立项, verbatim)
网页游戏, 在线5人, 暴力漂移赛车, 有道具的实时比赛, 全球积分记录到Supabase(免费档)。
用户可上传自己汽车的照片→在线生成3D车模→游戏中道具自动适配不同车型长出来。
免费系统自带车模; 不免费的需要用户看广告解锁。
3D生成平台: Tripo AI(免费200cr/月≈13车)首选, 本机TRELLIS-2/TripoSR兜底。

## 里程碑
- M1: 单机漂移Demo(Three.js物理漂移+一辆车+一条赛道) ← 现在干
- M2: 道具系统+5人联机(Supabase Realtime)+全球积分榜
- M3: 照片→3D车模管线(Tripo API)+车库+道具自动适配(包围盒挂点)
- M4: 广告解锁双轨上线

## 技术栈
- 客户端: Three.js + 自研漂移物理(参考nordschleife-racer 12.7k行)
- 联机: Supabase Realtime(免费档: 500 DB / 2GB带宽 / 200并发)
- 3D生成: Tripo API(M3) + TRELLIS-2本机兜底
- 部署: 静态托管(免费)
