# PC MHW Weapon Defense Cheats Tool CT
PC MONSTER HUNTER WORLD Weapon Defense Cheats Tool CT</br>
PC 怪物猎人 装备自定义修改 CT

<img src="https://i.imgur.com/VvOreGb.png" alt="MHW"/>
代码构架（每4位等于一格值 即00 00 00 00）：<br>
<table>
  <tbody>
    <tr>
      <td><div align="center">防具</div></td>
      <td><div align="center">防具部位</div></td>
      <td><div align="center">防具样式</div></td>
      <td><div align="center">防具等级</div></td>
      <td><div align="center">防具升级次数</div></td>
      <td><div align="center">装饰品1</div></td>
      <td><div align="center">装饰品2</div></td>
      <td><div align="center">装饰品3</div></td>
      <td><br></td>
      <td></td>
      <td><br></td>
      <td></td>
      <td><br></td>
      <td></td>
    </tr>
    <tr>
      <td><div align="center">武器</div></td>
      <td><div align="center">武器种类</div></td>
      <td><div align="center">武器样式</div></td>
      <td><br></td>
      <td></td>
      <td><div align="center">装饰品1</div></td>
      <td><div align="center">装饰品2</div></td>
      <td><div align="center">装饰品3</div></td>
      <td><div align="center">弩自定义强化1</div></td>
      <td><div align="center">弩自定义强化2</div></td>
      <td><div align="center">弩自定义强化3</div></td>
      <td><div align="center">自定义强化1</div></td>
      <td><div align="center">自定义强化2</div></td>
      <td><div align="center">自定义强化3</div></td>
    </tr>
    <tr>
      <td><div align="center">护石</div></td>
      <td><div align="center">护石固定ID 05</div></td>
      <td><div align="center">护石样式</div></td>
      <td><br></td>
      <td></td>
      <td><div align="center">装饰品1</div></td>
      <td><div align="center">装饰品2</div></td>
      <td><div align="center">装饰品3</div></td>
      <td><br></td>
      <td></td>
      <td><br></td>
      <td></td>
      <td><br></td>
      <td></td>
    </tr>
    <tr>
      <td><div align="center">猎虫</div></td>
      <td><div align="center">猎虫固定ID FF</div></td>
      <td><div align="center">猎虫样式</div></td>
      <td><br></td>
      <td></td>
      <td><br></td>
      <td></td>
      <td><br></td>
      <td></td>
      <td><br></td>
      <td></td>
      <td><br></td>
      <td></td>
      <td></td>
    </tr>
  </tbody>
</table>
其实知道这个武器种类和代码是多少用CE搜索 字节数组都能找到准确位置<br>
例如：太刀 的 天上天下無双刀 太刀种类ID=03 天上天下無双刀=59<br>
输入 03 00 00 00 59 00 00 00 搜索字节数组即可，一般得到几个结果，157749版本基本都在9开头位置里<br>
最后查看16进制代码去判断下一个武器是否是这个武器后获得的就行了<br>
代码的武器排序是获得时间排列，例如 天上天下無双刀 后面你做了个防具或者护石 就是对应的代码<br>

在装备只有一个孔或者只能自定义强化一次情况下可以使用本工具添加代码硬加珠子和强化项目都是有效的<br>
自行可以查看单个装备属性，是否有加珠子技能或者其他加成

装备总种类ID区分防具、武器、护石、猎虫，即00、01、02、04（03是未知会奔溃）<br>
防具等级只限防具有效，输入99实际上游戏显示LV100，当然也有100等级的防御，貌似没上限自行悠着点改<br>
自定义强化只限武器有效，如发现防具或护石里出现自定义强化数值请无视应该是某个固定值<br>
