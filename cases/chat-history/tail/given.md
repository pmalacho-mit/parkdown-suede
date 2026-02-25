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

... previous messages ...

<div data-src="../chats/*.md" data-sort="created" data-order="desc" data-processing="lifo" data-limit="2" data-template="tutor,user" data-join="\n\n-"></div>
