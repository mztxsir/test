###01-


###02-查看我的申请
```http request
https://manhattan.webapp.xiaojukeji.com/zeus/api/mine/query-credit-list?wsgsig=dd03-Rtjla6T4W0fJDTIXm%2F0dL2qNkXmN0OOXkkyA2OlIkXm%2BCS5pW9geM2w1Vgf%2BC6eVidu2NIU6VW4LdH2Zmeva1IxKU0c3fTVrn%2Fv915O7%2FXCKgTUin9De1IS2V0q
```
请求：
```json
{
	"pageIndex": 0,
	"pageSize": 10,
	"token": "-AeUaaEKlGRNDHD5o2g6dOwZCiPt_OTVN9kuMyGg2U0kzLltxEAMQNFefkwIPIaUh6lz9-BDPpIxYGMjQb1vsA28k6U0semmCMtoE5bTpqourKBtz-lTZw3LKmENWoWVNM8vCK80CG-0P8UYlm41c7oLH3QIB33y_3v7ez_oqaZxCZ-0ZYXvYTGFLxqLqFLPrET4frA_tF73AAAA__8="
}
```
响应：
```json
{
	"errorCode": 10000,
	"errorMsg": "成功",
	"data": {
		"hasMore": false,
		"creditList": [{
			"fundsChannelId": "3603",
			"creditLine": 1410000,
			"creditLineAvailable": 1310000,
			"interestRate": 972,
			"state": 1,
			"limitState": null,
			"applicationId": "DC000036032019071714f430c387b1",
			"applyTime": "2019-07-17 14:11:22"
		}]
	}
}
```
###02-我的申请-详情（只在app端有显示）




###点击还钱（默认是全部）：
url：
```http request
https://manhattan.webapp.xiaojukeji.com/zeus/api/repayment/loanlist?wsgsig=dd03-YoW1a2JNTgggWvTXVxQuMM04znncsyLXXZRT2Sb5znnbXuYpl6CYM64Mo0gbXKhVr2pkNMDHom3ah7xZUxfw1OG4pntajvxXUxnRLOKHugDfVKFt%2FxcQ%2B6KJug9
```
请求：
```json
{
	"pageSize": 10,
	"pageIndex": 1,
	"token": "-AeUaaEKlGRNDHD5o2g6dOwZCiPt_OTVN9kuMyGg2U0kzLltxEAMQNFefkwIPIaUh6lz9-BDPpIxYGMjQb1vsA28k6U0semmCMtoE5bTpqourKBtz-lTZw3LKmENWoWVNM8vCK80CG-0P8UYlm41c7oLH3QIB33y_3v7ez_oqaZxCZ-0ZYXvYTGFLxqLqFLPrET4frA_tF73AAAA__8="
}
```
响应：
```json
{
	"errorCode": 10000,
	"errorMsg": "成功",
	"data": {
		"withdrawList": [{
			"mobile": null,
			"bankCardName": "邮储银行",
			"interestRate": 0,
			"penaltyRate": 0,
			"loanOrderId": "DC000236032019071714220086e78a",
			"loanStatus": 1,
			"productId": "2018",
			"fundsChannelId": "3603",
			"curShouldPayAmount": 0,
			"shouldPayDate": "2019-08-17 00:00:00",
			"bankCardNo": "6221********5884",
			"isOverdue": false,
			"repayPlanList": null,
			"loanTimeInfo": {
				"loanStartTime": "2019-07-17 14:24:55",
				"loanEndTime": null,
				"loanIssueTime": null,
				"interestStartTime": null,
				"loanClearTime": null
			},
			"amountInfo": {
				"totalAmount": 100000,
				"principal": 100000,
				"interest": 0,
				"penalty": 0,
				"fee": 0
			},
			"totalDuration": 0,
			"failReason": null,
			"remark": null,
			"unpaidAmountInfo": null,
			"unReturnDiscountAmount": null,
			"couponName": null
		}],
		"hasMore": true
	}
}
```

###还钱：已还
```http request
https://manhattan.webapp.xiaojukeji.com/zeus/api/repayment/loanlist?wsgsig=dd03-gL2essmrJ8POxGKYJ8ehzfjk1zISZDQYH4dqQgoj1zITw07%2F3zxlyWXsI%2BPTwmguNv9ZxmzUHoUoQt4WJp6hzti%2FIJPOxGJPJ8ErymQh5%2BOyOWcyI8MjQGpsK%2B5
```

请求：
```json
{
	"LoanStatus": 3,
	"pageSize": 10,
	"pageIndex": 1,
	"token": "-AeUaaEKlGRNDHD5o2g6dOwZCiPt_OTVN9kuMyGg2U0kzLltxEAMQNFefkwIPIaUh6lz9-BDPpIxYGMjQb1vsA28k6U0semmCMtoE5bTpqourKBtz-lTZw3LKmENWoWVNM8vCK80CG-0P8UYlm41c7oLH3QIB33y_3v7ez_oqaZxCZ-0ZYXvYTGFLxqLqFLPrET4frA_tF73AAAA__8="
}
```

响应：
```json
{
	"errorCode": 10000,
	"errorMsg": "成功",
	"data": {
		"withdrawList": [],
		"hasMore": false
	}
}
```

###还钱：待还
```http request
https://manhattan.webapp.xiaojukeji.com/zeus/api/repayment/loanlist?wsgsig=dd03-Ymfe%2BPHfQEzgduI6VVWnaxBDYU8c9zO6Xr4q059EYU8bev5elFilcT2ePdzbeJe8rB8Z9xBcOliaD82DVlfkG62LPkR9B8H%2BU%2F0qb1BdREtdeQq%2BhFW%2FaxebOkL
```
请求：
```json
{
	"LoanStatus": 1,
	"pageSize": 10,
	"pageIndex": 1,
	"token": "-AeUaaEKlGRNDHD5o2g6dOwZCiPt_OTVN9kuMyGg2U0kzLltxEAMQNFefkwIPIaUh6lz9-BDPpIxYGMjQb1vsA28k6U0semmCMtoE5bTpqourKBtz-lTZw3LKmENWoWVNM8vCK80CG-0P8UYlm41c7oLH3QIB33y_3v7ez_oqaZxCZ-0ZYXvYTGFLxqLqFLPrET4frA_tF73AAAA__8="
}
```
响应：
```json

```

###我-我的银行卡
URL：
```http request
https://manhattan.webapp.xiaojukeji.com/zeus/api/bankcard/my-bank-cards?wsgsig=dd03-Aq1wTnMrAHLW6AyF6j98htAkbOSs2F8F8neIVCejbOSt5BRMMcw5hj5sD1Lt5%2Fs02ga9itEqC2BqJVo4HfE3%2FcPjgHLv5qbF7jd8VcduC1wuIlvd7t6%2BjWEVfO9
```

请求：
```json
{
	"token": "-AeUaaEKlGRNDHD5o2g6dOwZCiPt_OTVN9kuMyGg2U0kzLltxEAMQNFefkwIPIaUh6lz9-BDPpIxYGMjQb1vsA28k6U0semmCMtoE5bTpqourKBtz-lTZw3LKmENWoWVNM8vCK80CG-0P8UYlm41c7oLH3QIB33y_3v7ez_oqaZxCZ-0ZYXvYTGFLxqLqFLPrET4frA_tF73AAAA__8="
}

```

响应
```json
{
	"errorCode": 10000,
	"errorMsg": "成功",
	"data": {
		"cardInfoList": [{
			"bankName": "邮储银行",
			"bankCode": "0100",
			"bankLogo": "//manhattan.didistatic.com/static/manhattan/blanka_bank/uploads/3204b8a7a012c911853507a6718216a7",
			"originBankCode": "01000000",
			"bankStatus": null,
			"bankLimitDay": null,
			"bankLimitOnce": null,
			"bankLimitMonth": null,
			"defaultColor": "[\"#2FC6A9\",\"#28A991\"]",
			"commonBankAbbr": "PSBC",
			"cardType": 1,
			"cardTypeZh": "借记卡",
			"bankExtends": null,
			"bankCardNo": "6221********5884",
			"productId": "2018",
			"fundsChannelId": "3603"
		}],
		"bankCardCount": null
	}
}
```



20190718疑问：
参数的中文文档
create-repay中返回"验证码未获取或已失效"
//manhattan.webapp.xiaojukeji.com/zeus/api/repayment/create-repay，连发4次请求，每次返回都是成功，为什么
在每个http请求中最后的参数都带有wsgsig=***********，这串数据代表什么意思？
在请求体中都带有token，这个token中含有什么
fundsChannelId：3610是不是杭银消费？3603是不是马上消费金融股份有限公司？

在还款之前需要填写滴滴金融发送的验证码，在超时的情况下抓包会显示超时，但手机页面会提示还款申请已提交