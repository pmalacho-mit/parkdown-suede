# Chat History

<template id="msg">
({created|YYYY-MM-DDTHH:mm:ss.SSSZ}): {content|strip}
</template>

<template id="tutor" data-name-match="^tutor-\d+\.md$">
Tutor <span data-src="{path}" data-template="msg"></span>
</template>

<template id="user" data-name-match="^user-\d+\.md$">
User <span data-src="{path}" data-template="msg"></span>
</template>

<div data-src="../chats/*.md" data-sort="created" data-template="tutor,user" data-join="\n\n-">

User (2026-02-22T16:26:00.000Z): Hello.

Tutor (2026-02-22T16:26:05.000Z): Hi, I'm here to help.

User (2026-02-22T16:26:10.000Z): Thank you. What's your name?

Tutor (2026-02-22T16:26:15.000Z): I am an AI.

User (2026-02-22T16:26:20.000Z): Interesting.

Tutor (2026-02-22T16:26:25.000Z): Very.

</div>
