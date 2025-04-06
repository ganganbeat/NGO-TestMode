# NGO-TestMode
NEEDY GIRL OVERDOSEでテストモードに入るためのメモ

簡単に言うとWindow2DTestSceneを呼び出すだけ<br><br>
dnSpyでngov3.Bootで検索をかけて上にあるpublic void Awake()で右クリックしてEdit Method<br>

```
using System;
using System.Collections.Generic;
using Cysharp.Threading.Tasks;
using DG.Tweening;
using TMPro;
using UnityEngine;
using UnityEngine.UI;
using UnityEngine.SceneManagement;

namespace ngov3
{
	// Token: 0x020008BD RID: 2237
	public partial class Boot : MonoBehaviour
	{
		// Token: 0x06002621 RID: 9761 RVA: 0x00013F2E File Offset: 0x0001212E
		public void Awake()
		{
			SingletonMonoBehaviour<Settings>.Instance.saveNumber = 4;
			SceneManager.LoadScene("Window2DTestScene");
		}
	}
}
```
