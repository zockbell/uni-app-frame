<template>
    <view class="detailWrap">
        <image class="top" mode="widthFix" :src="detailOne.topImg"></image>
        <text class="title">{{detailOne.title}}</text>
        <view class="rich">
            <rich-text class="content" :nodes="detailOne.html"></rich-text>
        </view>
        <image class="top" mode="widthFix" :src="detailOne.bottomImg"></image>

        <!-- button -->
        <view class="share">
            <button type="warn" plain="true" open-type="share">分享给好友</button>
        </view>
    </view>
</template>

<script lang="ts">
	export default {
		data() {
			return {
                detailOne: null,
                detailData: [
                {
                    topImg: '/static/pic1.jpeg',
                    title: '西柏坡红色旅游区',
                    bottomImg: '/static/pic2.jpeg',
                    html: `
                    <p style="text-indent: 2em;">西柏坡红色旅游区为国家级风景名胜区、国家AAAAA级旅游景区、红色旅游经典景区、爱国主义教育基地。</p>
                    <br>

                    <p style="text-indent: 2em;">西柏坡位于河北省平山县中部，是解放战争时期中央工委、中共中央和解放军总部的所在地。1947年5月，刘少奇、朱德率中央工委进驻西柏坡。1948年5月，毛泽东、周恩来、任弼时率中央前委和解放军总部到西柏坡与中央工委汇合。在这里，毛泽东和他的战友们召开了中国共产党全国土地会议，通过了《中国土地法大纲》，实现了耕者有其田；指挥了辽沈、淮海、平津三大战役，决定了中国的命运；召开了中国共产党七届二中全会，描绘了新中国宏伟的蓝图。1949年3月23日，中共中央和解放军总部离开西柏坡，赴京建国。新中国从这里走来。</p>
                    <br>

                    <p style="text-indent: 2em;">中共中央离开后，留守人员与建屏县政府(1958年改为平山县)对中央机关留下的东西进行了交接。为了保护革命遗址和文物，1955年，河北省博物馆联合当地政府建立了西柏坡纪念馆筹备处。1958年因修建岗南水库，将中共中央旧址搬迁。1970年12月开始，在距原址北移500米，海拔升高57米的地方进行易地复原建设。1982年3月11日，国务院公布西柏坡中共中央旧址为全国重点文物保护单位。1987年5月1日，立文物保护区碑一座，划定文物保护区391800平方米，自然保护区1333200平方米。</p>

                    <br>

                    <p style="text-indent: 2em;">西柏坡陈列展览馆于1976年10月开工。1978年5月26日纪念中共中央和解放军总部移驻西柏坡30周年时与中共中央旧址同时对外开放。主题陈列《新中国从这里走来》曾于1993年、1996年、1998年、2003年、2009年进行了修改完善，曾被国家文物局评为“1998年度全国十大精品陈列”。第六届（2003至2004年度）全国十大陈列展览特别奖。</p>
                    <br>

                    <p style="text-indent: 2em;">1992年开始新修建了西柏坡石刻园（2011年扩建改名为西柏坡丰碑林）、西柏坡雕塑园、五大书记铜铸像、西柏坡纪念碑、周恩来评语碑、西柏坡教育馆、西柏坡文物保护碑、西柏坡青少年文明园、西柏坡廉政教育馆等革命传统教育系列工程，极大地丰富了西柏坡纪念馆的教育内容。</p>
                    `,
                },
                {
                    topImg: '/static/pic2.gif',
                    title: '井陉万人坑纪念馆',
                    bottomImg: '/static/pic5.jpeg',
                    html: `
                    <p style="text-indent: 2em;">矿区万人坑一共六座。在旧社会约有4.6万死难矿工被集中丢弃在这6座万人坑中。其中，南大沟万人坑持续时间最长，丢弃的死难矿工最多。万人坑纪念馆以灰色为主色调，采用内外景协调一致的设计手法，追求形式与内容的统一。它以独特的建筑语言——弧线与斜面，构造主建筑外形及魂坡、魂墙，巧妙地诠释着陈展主题，是精美的建筑佳作。</p>
                    <br>

                    <p style="text-indent: 2em;">南大沟万人坑遗址年代为1899—1947年，位于石家庄市井陉矿区。 2008年10月20日南大沟万人坑遗址被河北省人民政府公布为第五批省级文物保护单位。</p>
                    <br>

                    <p style="text-indent: 2em;">在井陉矿区“万人坑”遗址附近还有百团大战中央纵队指挥所旧址、日本小姑娘美穗子姐妹获救处、延安（陕北）新华广播电台旧址、华北大学工业园旧址、晋察冀边区工业局旧址、二十号“阎王殿”、井陉矿南井和皇冠水塔等一些集教育、文化、旅游于一体的旧址、遗址，都是井陉矿区爱国主义教育基地的重要组成部分。</p>
                    `,
                },
                {
                    topImg: '/static/pic3.gif',
                    title: '梅花惨案纪念馆',
                    bottomImg: '/static/pic6.jpeg',
                    html: `
                    <p style="text-indent: 2em;">梅花惨案纪念馆位于河北省藁城市市区正南20公里处的梅花镇，1982年河北省人民政府将其公布为河北省重点文物保护单位，1994年又被河北省政府批准为省级爱国主义教育基地。</p>
                    <br>

                    <p style="text-indent: 2em;">梅花自古以来就是闻名华北的商业重镇。“七七事变”后，日本侵略军长驱直入，疯狂南侵。1937年10月11日，原国民党53军691团。在团长吕正操(已加入中国共产党)率领下，高举抗日救国的旗帜，在梅花村英勇阻击入侵日军，共打死打伤日军800多名，打破了“皇军”不可战胜的神话。</p>
                    <br>

                    <p style="text-indent: 2em;">10月12日夜(农历九月初九)，日本侵略军占领梅花，展开血腥大-，共杀害我同胞1547人，占当时全村人口的60%，杀绝46户，烧毁房屋600多间。妇女儿童也未能幸免，村民尸体布满了大街小巷，残尸断肢随地可见，鲜血流遍了整个村镇。日寇四天三夜的烧杀-，使这里变成了处处残垣断壁，家家戴孝埋人的人间地狱。这就是骇人听闻的“九九梅花惨案”。</p>

                    <br>

                    <p style="text-indent: 2em;">新中国成立后，党和政府在梅花村相继修建了殉国烈士亭、纪念碑，保存下来四处较大的惨案遗址——辘轳把水坑、碱水坑、血井、三十六口坟，成为爱国主义教育基地。</p>

                    <br>

                    <p style="text-indent: 2em;">梅花惨案纪念馆始建于1958年，1996年8月因特大洪水全部倒塌。1998年2月经省爱国主义教育基地领导小组批准，总投资350多万元进行了重建。基地由北院、南院和村西辘轳把水坑遗址三部分组成，占地27.9亩，总建筑面积736平方米。北院、南院隔路对置。座北朝南的梅花惨案纪念馆位于北院正中央，面积576平方米，为一正方形建筑。馆中间高出6米的半球体，寓意“神州陆沉”，纪念馆正门上方由原全国政协副主席吕正操同志题写的“梅花惨案纪念馆”馆名。北院大门是两个大写的“九”字，相对而立，示意着惨案发生的时间(农历九月初九)。展厅中央为高2.35米的铜雕，其后是一座长7.02米，高2.65米的巨型浮雕。四面是“沃野明珠”、“铁狮怒吼”、“九九血证”、“历史昭示”的环形展览。展厅内还配置了VCD及背投电视,以播放与惨案有关的资料、物证、人证等纪录片。</p>

                    `,
                }
                ]
			}
		},
		onLoad(options) {
            // console.log(options);
            switch(options.id) {
            case '1':
                this.detailOne = this.detailData[0]
                break;
            case '2':
                this.detailOne = this.detailData[1]
                break;
            case '3':
                this.detailOne = this.detailData[2]
                break;
            }
		},
		methods: {
		}
	}
</script>

<style scoped>
.detailWrap {
  padding-bottom: 10px;
}

.top {
  width: 100%;
}

.title {
  margin: 15px;
  display: block;
  font-size: 20px;
  line-height: 20px;
  text-align: center;
}

.rich {
  margin: 15px;
}

.content {
  color: #666;
  line-height: 2;
  font-size: 16px;
}

.rich img {
  width: 100%;
}

.share {
  margin: 15px 15px 30px;
}
</style>