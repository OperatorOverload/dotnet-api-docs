all: server.exe client.exe

server.exe: ChannelServices_registeredchannels_Server.vb ChannelServices_registeredchannels_Share.dll
	vbc ChannelServices_registeredchannels_Server.vb /r:ChannelServices_registeredchannels_Share.dll

client.exe: channelservices_registeredchannels_client.vb ChannelServices_registeredchannels_Share.dll
	vbc ChannelServices_registeredchannels_client.vb /r:ChannelServices_registeredchannels_Share.dll

ChannelServices_RegisteredChannels_Share.dll: ChannelServices_RegisteredChannels_Share.vb
	vbc /t:library ChannelServices_RegisteredChannels_Share.vb
