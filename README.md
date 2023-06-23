Run the rulebook:

```
export BOT_ID=xxx
ansible-rulebook --rulebook rulebooks/listen-groupme.yml -i inventory/hosts.yml -E BOT_ID
```

Sample payload:

```
{
    'payload':
    {
    'attachments': [],
    'source_guid': 'e9616c30f3b7013bc44f6ab22d456705',
    'system': False,
    'avatar_url': 'https://i.groupme.com/460x460.png.a80dd4561cc9458bb5d2dd7b8c18f65b',
    'group_id': 'xxxxxxxx',
    'user_id': 'xxxxxx',
    'sender_type': 'bot',
    'name': 'EDA Chatbot',
    'created_at': 1687499484,
    'id': 'xxxxxxxxxxxxxxxxxx',
    'text': 'Hello world!',
    'sender_id': 'xxxxxx'},
    'meta':
    {
        'headers':
        {
            'User-Agent': 'GroupMeBotNotifier/1.0',
            'Connection': 'close',
            'Host': 'chatbot.escwq.xyz:5000',
            'Accept-Encoding': 'gzip',
            'Content-Length': '339',
            'Content-Type': 'application/json'
        },
        'endpoint': '',
        'received_at': '2023-06-23T05:51:24.741568Z',
        'source':
        {
            'name': 'ansible.eda.webhook',
            'type': 'ansible.eda.webhook'
        },
        'uuid': '00d7736f-d0d2-4955-b5aa-b28415cab34a'
    }
}
```
