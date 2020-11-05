set(COMPONENT_NAME "MQTTPacket")
set(COMPONENT_ADD_INCLUDEDIRS "src src/mbedtls")
set(COMPONENT_INCLUDEDIRS "src src/mbedtls")
set(COMPONENT_PRIV_INCLUDEDIRS "src src/mbedtls")
set(mqttpacket_sdk_dir src)
set(COMPONENT_SRCS "${mqttpacket_sdk_dir}/MQTTConnectClient.c"
                    "${mqttpacket_sdk_dir}/MQTTConnectServer.c"
                    "${mqttpacket_sdk_dir}/MQTTSerializePublish.c"
                    "${mqttpacket_sdk_dir}/MQTTDeserializePublish.c"
                    "${mqttpacket_sdk_dir}/MQTTFormat.c"
                    "${mqttpacket_sdk_dir}/MQTTPacket.c"                    
                    "${mqttpacket_sdk_dir}/MQTTSubscribeClient.c"
                    "${mqttpacket_sdk_dir}/MQTTUnsubscribeClient.c"
                    "${mqttpacket_sdk_dir}/MQTTUnsubscribeServer.c"
                    "${mqttpacket_sdk_dir}/MQTTClient.c"
                    "${mqttpacket_sdk_dir}/mbedtls/MQTTmbedtls.c")
set(COMPONENT_REQUIRES "mbedtls")
register_component()