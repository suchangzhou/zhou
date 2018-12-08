# zhou
dingtalk
# -*- coding: gbk -*

import requests
import json
url='https://oapi.dingtalk.com/robot/send?access_token=1e0b52ba466cfbbde8db90577900847421b03aada4ef2cf4098d00dc083b493f'
program={
"msgtype": "text",
"text": {"content": "测试！"},
}
headers={'Content-Type': 'application/json'}
f=requests.post(url,data=json.dumps(program),headers=headers)
