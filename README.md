# Codigo-Avatar-Discord.js-V.12
Para la versión 12


//CODIGO AVATAR

client.on("message", message => {
if (message.content.startsWith(prefix + "avatar" )){
let miembro = message.mentions.users.first()
Bot: if(message.author.bot) return;

if (!miembro) {
    const embed = new Discord.MessageEmbed()
        .setImage(`${message.author.displayAvatarURL()}`)
        .setColor(0x66b3ff)
        .setTimestamp()
    message.channel.send(embed);

} else {
    const embed = new Discord.MessageEmbed()
        .setImage(`${miembro.displayAvatarURL()}`)
        .setColor(0x66b33f)

        .setTimestamp()

    message.channel.send(embed);

};
};
});
