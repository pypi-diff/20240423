# Comparing `tmp/socket.d-2.4.10.7.tar.gz` & `tmp/socket.d-2.4.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socket.d-2.4.10.7.tar", last modified: Fri Apr 19 01:42:40 2024, max compression
+gzip compressed data, was "socket.d-2.4.11.tar", last modified: Tue Apr 23 02:53:54 2024, max compression
```

## Comparing `socket.d-2.4.10.7.tar` & `socket.d-2.4.11.tar`

### file list

```diff
@@ -1,149 +1,153 @@
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-19 01:42:40.928570 socket.d-2.4.10.7/
--rw-r--r--   0 noear      (501) staff       (20)      555 2024-04-19 01:42:40.927819 socket.d-2.4.10.7/PKG-INFO
--rw-r--r--   0 noear      (501) staff       (20)     1713 2024-04-18 04:06:21.000000 socket.d-2.4.10.7/README.md
--rw-r--r--   0 noear      (501) staff       (20)       38 2024-04-19 01:42:40.928770 socket.d-2.4.10.7/setup.cfg
--rw-r--r--   0 noear      (501) staff       (20)      875 2024-04-19 01:42:14.000000 socket.d-2.4.10.7/setup.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-19 01:42:40.926874 socket.d-2.4.10.7/socket.d.egg-info/
--rw-r--r--   0 noear      (501) staff       (20)      555 2024-04-19 01:42:40.000000 socket.d-2.4.10.7/socket.d.egg-info/PKG-INFO
--rw-r--r--   0 noear      (501) staff       (20)     4924 2024-04-19 01:42:40.000000 socket.d-2.4.10.7/socket.d.egg-info/SOURCES.txt
--rw-r--r--   0 noear      (501) staff       (20)        1 2024-04-19 01:42:40.000000 socket.d-2.4.10.7/socket.d.egg-info/dependency_links.txt
--rw-r--r--   0 noear      (501) staff       (20)       18 2024-04-19 01:42:40.000000 socket.d-2.4.10.7/socket.d.egg-info/requires.txt
--rw-r--r--   0 noear      (501) staff       (20)       42 2024-04-19 01:42:40.000000 socket.d-2.4.10.7/socket.d.egg-info/top_level.txt
--rw-r--r--   0 noear      (501) staff       (20)        1 2024-04-19 01:42:40.000000 socket.d-2.4.10.7/socket.d.egg-info/zip-safe
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-19 01:42:40.842239 socket.d-2.4.10.7/socketd/
--rw-r--r--   0 noear      (501) staff       (20)     4162 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/SocketD.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-19 01:42:40.845366 socket.d-2.4.10.7/socketd/broker/
--rw-r--r--   0 noear      (501) staff       (20)      243 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/broker/BrokerFragmentHandler.py
--rw-r--r--   0 noear      (501) staff       (20)     3571 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/broker/BrokerListener.py
--rw-r--r--   0 noear      (501) staff       (20)     3134 2024-04-19 01:32:01.000000 socket.d-2.4.10.7/socketd/broker/BrokerListenerBase.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/broker/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-19 01:42:40.847965 socket.d-2.4.10.7/socketd/cluster/
--rw-r--r--   0 noear      (501) staff       (20)     2757 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/cluster/ClusterClient.py
--rw-r--r--   0 noear      (501) staff       (20)     2700 2024-04-19 01:32:01.000000 socket.d-2.4.10.7/socketd/cluster/ClusterClientSession.py
--rw-r--r--   0 noear      (501) staff       (20)     2005 2024-04-19 01:32:01.000000 socket.d-2.4.10.7/socketd/cluster/LoadBalancer.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/cluster/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-19 01:42:40.849863 socket.d-2.4.10.7/socketd/exception/
--rw-r--r--   0 noear      (501) staff       (20)      654 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/exception/SocketDExecption.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/exception/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-19 01:42:40.850391 socket.d-2.4.10.7/socketd/transport/
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-19 01:42:40.859969 socket.d-2.4.10.7/socketd/transport/client/
--rw-r--r--   0 noear      (501) staff       (20)     1720 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/client/Client.py
--rw-r--r--   0 noear      (501) staff       (20)     3607 2024-04-18 09:13:43.000000 socket.d-2.4.10.7/socketd/transport/client/ClientBase.py
--rw-r--r--   0 noear      (501) staff       (20)     6520 2024-04-18 09:13:43.000000 socket.d-2.4.10.7/socketd/transport/client/ClientChannel.py
--rw-r--r--   0 noear      (501) staff       (20)     2843 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/client/ClientConfig.py
--rw-r--r--   0 noear      (501) staff       (20)      144 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/client/ClientConfigHandler.py
--rw-r--r--   0 noear      (501) staff       (20)      384 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/client/ClientConnectHandler.py
--rw-r--r--   0 noear      (501) staff       (20)      483 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/client/ClientConnector.py
--rw-r--r--   0 noear      (501) staff       (20)      462 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/client/ClientConnectorBase.py
--rw-r--r--   0 noear      (501) staff       (20)      373 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/client/ClientHandshakeResult.py
--rw-r--r--   0 noear      (501) staff       (20)      224 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/client/ClientHeartbeatHandler.py
--rw-r--r--   0 noear      (501) staff       (20)      303 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/client/ClientProvider.py
--rw-r--r--   0 noear      (501) staff       (20)     1126 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/client/ClientSession.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/client/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-19 01:42:40.877666 socket.d-2.4.10.7/socketd/transport/core/
--rw-r--r--   0 noear      (501) staff       (20)     1426 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/core/Asserts.py
--rw-r--r--   0 noear      (501) staff       (20)     2482 2024-04-18 09:13:43.000000 socket.d-2.4.10.7/socketd/transport/core/Channel.py
--rw-r--r--   0 noear      (501) staff       (20)      688 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/core/ChannelAssistant.py
--rw-r--r--   0 noear      (501) staff       (20)      625 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/core/ChannelInternal.py
--rw-r--r--   0 noear      (501) staff       (20)      517 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/core/ChannelSupporter.py
--rw-r--r--   0 noear      (501) staff       (20)     1294 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/core/Codec.py
--rw-r--r--   0 noear      (501) staff       (20)     2978 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/core/Config.py
--rw-r--r--   0 noear      (501) staff       (20)     1262 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/core/Costants.py
--rw-r--r--   0 noear      (501) staff       (20)     1148 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/core/Entity.py
--rw-r--r--   0 noear      (501) staff       (20)      697 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/core/EntityMetas.py
--rw-r--r--   0 noear      (501) staff       (20)     1717 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/core/Flags.py
--rw-r--r--   0 noear      (501) staff       (20)     1154 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/core/FragmentAggregator.py
--rw-r--r--   0 noear      (501) staff       (20)      838 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/core/FragmentHandler.py
--rw-r--r--   0 noear      (501) staff       (20)      419 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/core/Frame.py
--rw-r--r--   0 noear      (501) staff       (20)     2290 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/core/Frames.py
--rw-r--r--   0 noear      (501) staff       (20)     2536 2024-04-19 01:32:01.000000 socket.d-2.4.10.7/socketd/transport/core/HandshakeDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      170 2024-04-19 01:32:01.000000 socket.d-2.4.10.7/socketd/transport/core/IdGenerator.py
--rw-r--r--   0 noear      (501) staff       (20)      504 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/core/Listener.py
--rw-r--r--   0 noear      (501) staff       (20)      735 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/core/Message.py
--rw-r--r--   0 noear      (501) staff       (20)      801 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/core/Processor.py
--rw-r--r--   0 noear      (501) staff       (20)     1953 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/core/Session.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/core/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-19 01:42:40.880352 socket.d-2.4.10.7/socketd/transport/core/codec/
--rw-r--r--   0 noear      (501) staff       (20)     1164 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/core/codec/Buffer.py
--rw-r--r--   0 noear      (501) staff       (20)      780 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/core/codec/ByteBufferCodecReader.py
--rw-r--r--   0 noear      (501) staff       (20)      642 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/core/codec/ByteBufferCodecWriter.py
--rw-r--r--   0 noear      (501) staff       (20)     4514 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/core/codec/CodecDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      200 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/core/codec/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-19 01:42:40.885577 socket.d-2.4.10.7/socketd/transport/core/entity/
--rw-r--r--   0 noear      (501) staff       (20)     3783 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/core/entity/EntityDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      800 2024-04-18 13:46:31.000000 socket.d-2.4.10.7/socketd/transport/core/entity/FileEntity.py
--rw-r--r--   0 noear      (501) staff       (20)      885 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/core/entity/MessageBuilder.py
--rw-r--r--   0 noear      (501) staff       (20)     2045 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/core/entity/MessageDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      215 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/core/entity/StringEntity.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/core/entity/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-19 01:42:40.888875 socket.d-2.4.10.7/socketd/transport/core/fragment/
--rw-r--r--   0 noear      (501) staff       (20)     2010 2024-04-19 01:32:01.000000 socket.d-2.4.10.7/socketd/transport/core/fragment/FragmentAggregatorDefault.py
--rw-r--r--   0 noear      (501) staff       (20)     3377 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/core/fragment/FragmentHandlerBase.py
--rw-r--r--   0 noear      (501) staff       (20)      502 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/core/fragment/FragmentHandlerDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      188 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/core/fragment/FragmentHolder.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/core/fragment/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-19 01:42:40.894840 socket.d-2.4.10.7/socketd/transport/core/impl/
--rw-r--r--   0 noear      (501) staff       (20)     2358 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/core/impl/ChannelBase.py
--rw-r--r--   0 noear      (501) staff       (20)     6927 2024-04-18 09:13:43.000000 socket.d-2.4.10.7/socketd/transport/core/impl/ChannelDefault.py
--rw-r--r--   0 noear      (501) staff       (20)     6579 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/core/impl/ConfigBase.py
--rw-r--r--   0 noear      (501) staff       (20)      338 2024-04-18 09:13:43.000000 socket.d-2.4.10.7/socketd/transport/core/impl/LogConfig.py
--rw-r--r--   0 noear      (501) staff       (20)     7672 2024-04-18 09:13:43.000000 socket.d-2.4.10.7/socketd/transport/core/impl/ProcessorDefault.py
--rw-r--r--   0 noear      (501) staff       (20)     1355 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/core/impl/SessionBase.py
--rw-r--r--   0 noear      (501) staff       (20)     4288 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/core/impl/SessionDefault.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/core/impl/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-19 01:42:40.899676 socket.d-2.4.10.7/socketd/transport/core/listener/
--rw-r--r--   0 noear      (501) staff       (20)     2242 2024-04-18 11:54:48.000000 socket.d-2.4.10.7/socketd/transport/core/listener/EventListener.py
--rw-r--r--   0 noear      (501) staff       (20)     1043 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/core/listener/PathListener.py
--rw-r--r--   0 noear      (501) staff       (20)      176 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/core/listener/PathMapper.py
--rw-r--r--   0 noear      (501) staff       (20)      457 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/core/listener/PipelineListener.py
--rw-r--r--   0 noear      (501) staff       (20)      457 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/core/listener/SimpleListener.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/core/listener/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-19 01:42:40.903469 socket.d-2.4.10.7/socketd/transport/server/
--rw-r--r--   0 noear      (501) staff       (20)      723 2024-04-18 05:45:29.000000 socket.d-2.4.10.7/socketd/transport/server/Server.py
--rw-r--r--   0 noear      (501) staff       (20)     2437 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/server/ServerBase.py
--rw-r--r--   0 noear      (501) staff       (20)     1645 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/server/ServerConfig.py
--rw-r--r--   0 noear      (501) staff       (20)      250 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/server/ServerProvider.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/server/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-19 01:42:40.910086 socket.d-2.4.10.7/socketd/transport/stream/
--rw-r--r--   0 noear      (501) staff       (20)     1355 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/stream/RequestStream.py
--rw-r--r--   0 noear      (501) staff       (20)      332 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/stream/SendStream.py
--rw-r--r--   0 noear      (501) staff       (20)      690 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/stream/Stream.py
--rw-r--r--   0 noear      (501) staff       (20)     2100 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/stream/StreamBase.py
--rw-r--r--   0 noear      (501) staff       (20)      907 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/stream/StreamManger.py
--rw-r--r--   0 noear      (501) staff       (20)     1025 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/stream/StreamMangerDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      843 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/stream/SubscribeStream.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/stream/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-19 01:42:40.912496 socket.d-2.4.10.7/socketd/transport/utils/
--rw-r--r--   0 noear      (501) staff       (20)     3492 2024-04-19 01:32:01.000000 socket.d-2.4.10.7/socketd/transport/utils/AsyncUtils.py
--rw-r--r--   0 noear      (501) staff       (20)     1989 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/utils/CompletableFuture.py
--rw-r--r--   0 noear      (501) staff       (20)      665 2024-04-19 01:32:01.000000 socket.d-2.4.10.7/socketd/transport/utils/StrUtils.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/utils/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-19 01:42:40.913450 socket.d-2.4.10.7/socketd/transport/utils/async_api/
--rw-r--r--   0 noear      (501) staff       (20)      787 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/utils/async_api/AtomicRefer.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/utils/async_api/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-19 01:42:40.914265 socket.d-2.4.10.7/socketd/transport/utils/sync_api/
--rw-r--r--   0 noear      (501) staff       (20)      747 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/utils/sync_api/AtomicRefer.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd/transport/utils/sync_api/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-19 01:42:40.919351 socket.d-2.4.10.7/socketd_aio_tcp/
--rw-r--r--   0 noear      (501) staff       (20)     4144 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd_aio_tcp/TCPAIOServer.py
--rw-r--r--   0 noear      (501) staff       (20)      517 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd_aio_tcp/TCPStreamIO.py
--rw-r--r--   0 noear      (501) staff       (20)     2331 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd_aio_tcp/TcpAIOChannelAssistant.py
--rw-r--r--   0 noear      (501) staff       (20)      645 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd_aio_tcp/TcpAioClient.py
--rw-r--r--   0 noear      (501) staff       (20)     6597 2024-04-19 01:32:01.000000 socket.d-2.4.10.7/socketd_aio_tcp/TcpAioClientConnector.py
--rw-r--r--   0 noear      (501) staff       (20)      776 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd_aio_tcp/TcpAioProvider.py
--rw-r--r--   0 noear      (501) staff       (20)      183 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd_aio_tcp/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-19 01:42:40.922248 socket.d-2.4.10.7/socketd_websocket/
--rw-r--r--   0 noear      (501) staff       (20)     2471 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd_websocket/WsAioChannelAssistant.py
--rw-r--r--   0 noear      (501) staff       (20)      574 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd_websocket/WsAioClient.py
--rw-r--r--   0 noear      (501) staff       (20)     3639 2024-04-19 01:32:01.000000 socket.d-2.4.10.7/socketd_websocket/WsAioClientConnector.py
--rw-r--r--   0 noear      (501) staff       (20)      830 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd_websocket/WsAioProvider.py
--rw-r--r--   0 noear      (501) staff       (20)     2289 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd_websocket/WsAioServer.py
--rw-r--r--   0 noear      (501) staff       (20)      117 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd_websocket/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-19 01:42:40.926252 socket.d-2.4.10.7/socketd_websocket/impl/
--rw-r--r--   0 noear      (501) staff       (20)     4784 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd_websocket/impl/AIOConnect.py
--rw-r--r--   0 noear      (501) staff       (20)     6180 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd_websocket/impl/AIOServe.py
--rw-r--r--   0 noear      (501) staff       (20)     5990 2024-04-18 09:13:43.000000 socket.d-2.4.10.7/socketd_websocket/impl/AIOWebSocketClientImpl.py
--rw-r--r--   0 noear      (501) staff       (20)     4602 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd_websocket/impl/AIOWebSocketServerImpl.py
--rw-r--r--   0 noear      (501) staff       (20)      274 2024-04-18 02:59:52.000000 socket.d-2.4.10.7/socketd_websocket/impl/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.160510 socket.d-2.4.11/
+-rw-r--r--   0 noear      (501) staff       (20)      553 2024-04-23 02:53:54.159715 socket.d-2.4.11/PKG-INFO
+-rw-r--r--   0 noear      (501) staff       (20)     1713 2024-04-18 04:06:21.000000 socket.d-2.4.11/README.md
+-rw-r--r--   0 noear      (501) staff       (20)       38 2024-04-23 02:53:54.160696 socket.d-2.4.11/setup.cfg
+-rw-r--r--   0 noear      (501) staff       (20)      873 2024-04-23 02:26:11.000000 socket.d-2.4.11/setup.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.158442 socket.d-2.4.11/socket.d.egg-info/
+-rw-r--r--   0 noear      (501) staff       (20)      553 2024-04-23 02:53:53.000000 socket.d-2.4.11/socket.d.egg-info/PKG-INFO
+-rw-r--r--   0 noear      (501) staff       (20)     5025 2024-04-23 02:53:53.000000 socket.d-2.4.11/socket.d.egg-info/SOURCES.txt
+-rw-r--r--   0 noear      (501) staff       (20)        1 2024-04-23 02:53:53.000000 socket.d-2.4.11/socket.d.egg-info/dependency_links.txt
+-rw-r--r--   0 noear      (501) staff       (20)       18 2024-04-23 02:53:53.000000 socket.d-2.4.11/socket.d.egg-info/requires.txt
+-rw-r--r--   0 noear      (501) staff       (20)       42 2024-04-23 02:53:53.000000 socket.d-2.4.11/socket.d.egg-info/top_level.txt
+-rw-r--r--   0 noear      (501) staff       (20)        1 2024-04-23 02:53:53.000000 socket.d-2.4.11/socket.d.egg-info/zip-safe
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.009590 socket.d-2.4.11/socketd/
+-rw-r--r--   0 noear      (501) staff       (20)     4162 2024-04-23 02:26:11.000000 socket.d-2.4.11/socketd/SocketD.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.013870 socket.d-2.4.11/socketd/broker/
+-rw-r--r--   0 noear      (501) staff       (20)      243 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/broker/BrokerFragmentHandler.py
+-rw-r--r--   0 noear      (501) staff       (20)     3571 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/broker/BrokerListener.py
+-rw-r--r--   0 noear      (501) staff       (20)     3124 2024-04-23 02:49:12.000000 socket.d-2.4.11/socketd/broker/BrokerListenerBase.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/broker/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.017166 socket.d-2.4.11/socketd/cluster/
+-rw-r--r--   0 noear      (501) staff       (20)     2757 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/cluster/ClusterClient.py
+-rw-r--r--   0 noear      (501) staff       (20)     2690 2024-04-23 02:49:12.000000 socket.d-2.4.11/socketd/cluster/ClusterClientSession.py
+-rw-r--r--   0 noear      (501) staff       (20)     1995 2024-04-23 02:49:12.000000 socket.d-2.4.11/socketd/cluster/LoadBalancer.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/cluster/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.018444 socket.d-2.4.11/socketd/exception/
+-rw-r--r--   0 noear      (501) staff       (20)      654 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/exception/SocketDExecption.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/exception/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.019139 socket.d-2.4.11/socketd/transport/
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.031843 socket.d-2.4.11/socketd/transport/client/
+-rw-r--r--   0 noear      (501) staff       (20)     1720 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/client/Client.py
+-rw-r--r--   0 noear      (501) staff       (20)     3607 2024-04-18 09:13:43.000000 socket.d-2.4.11/socketd/transport/client/ClientBase.py
+-rw-r--r--   0 noear      (501) staff       (20)     6520 2024-04-23 02:48:32.000000 socket.d-2.4.11/socketd/transport/client/ClientChannel.py
+-rw-r--r--   0 noear      (501) staff       (20)     2843 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/client/ClientConfig.py
+-rw-r--r--   0 noear      (501) staff       (20)      144 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/client/ClientConfigHandler.py
+-rw-r--r--   0 noear      (501) staff       (20)      384 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/client/ClientConnectHandler.py
+-rw-r--r--   0 noear      (501) staff       (20)      483 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/client/ClientConnector.py
+-rw-r--r--   0 noear      (501) staff       (20)      462 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/client/ClientConnectorBase.py
+-rw-r--r--   0 noear      (501) staff       (20)      373 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/client/ClientHandshakeResult.py
+-rw-r--r--   0 noear      (501) staff       (20)      224 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/client/ClientHeartbeatHandler.py
+-rw-r--r--   0 noear      (501) staff       (20)      303 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/client/ClientProvider.py
+-rw-r--r--   0 noear      (501) staff       (20)     1126 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/client/ClientSession.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/client/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.051133 socket.d-2.4.11/socketd/transport/core/
+-rw-r--r--   0 noear      (501) staff       (20)     1426 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/Asserts.py
+-rw-r--r--   0 noear      (501) staff       (20)     2482 2024-04-18 09:13:43.000000 socket.d-2.4.11/socketd/transport/core/Channel.py
+-rw-r--r--   0 noear      (501) staff       (20)      688 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/ChannelAssistant.py
+-rw-r--r--   0 noear      (501) staff       (20)      625 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/ChannelInternal.py
+-rw-r--r--   0 noear      (501) staff       (20)      517 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/ChannelSupporter.py
+-rw-r--r--   0 noear      (501) staff       (20)     1355 2024-04-22 15:28:49.000000 socket.d-2.4.11/socketd/transport/core/Codec.py
+-rw-r--r--   0 noear      (501) staff       (20)     2978 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/Config.py
+-rw-r--r--   0 noear      (501) staff       (20)     1262 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/Costants.py
+-rw-r--r--   0 noear      (501) staff       (20)     1148 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/Entity.py
+-rw-r--r--   0 noear      (501) staff       (20)      697 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/EntityMetas.py
+-rw-r--r--   0 noear      (501) staff       (20)     1717 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/Flags.py
+-rw-r--r--   0 noear      (501) staff       (20)     1154 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/FragmentAggregator.py
+-rw-r--r--   0 noear      (501) staff       (20)      838 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/FragmentHandler.py
+-rw-r--r--   0 noear      (501) staff       (20)      419 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/Frame.py
+-rw-r--r--   0 noear      (501) staff       (20)     2290 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/Frames.py
+-rw-r--r--   0 noear      (501) staff       (20)     2526 2024-04-23 02:49:12.000000 socket.d-2.4.11/socketd/transport/core/HandshakeDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      160 2024-04-23 02:49:12.000000 socket.d-2.4.11/socketd/transport/core/IdGenerator.py
+-rw-r--r--   0 noear      (501) staff       (20)      510 2024-04-22 17:01:30.000000 socket.d-2.4.11/socketd/transport/core/Listener.py
+-rw-r--r--   0 noear      (501) staff       (20)      735 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/Message.py
+-rw-r--r--   0 noear      (501) staff       (20)      953 2024-04-23 00:58:23.000000 socket.d-2.4.11/socketd/transport/core/Processor.py
+-rw-r--r--   0 noear      (501) staff       (20)     1953 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/Session.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.056171 socket.d-2.4.11/socketd/transport/core/codec/
+-rw-r--r--   0 noear      (501) staff       (20)     1346 2024-04-22 15:48:56.000000 socket.d-2.4.11/socketd/transport/core/codec/Buffer.py
+-rw-r--r--   0 noear      (501) staff       (20)      777 2024-04-22 15:21:21.000000 socket.d-2.4.11/socketd/transport/core/codec/ByteBufferCodecReader.py
+-rw-r--r--   0 noear      (501) staff       (20)      666 2024-04-22 16:12:25.000000 socket.d-2.4.11/socketd/transport/core/codec/ByteBufferCodecWriter.py
+-rw-r--r--   0 noear      (501) staff       (20)     4634 2024-04-22 16:02:45.000000 socket.d-2.4.11/socketd/transport/core/codec/CodecDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      200 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/codec/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.062763 socket.d-2.4.11/socketd/transport/core/entity/
+-rw-r--r--   0 noear      (501) staff       (20)     3783 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/entity/EntityDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      800 2024-04-18 13:46:31.000000 socket.d-2.4.11/socketd/transport/core/entity/FileEntity.py
+-rw-r--r--   0 noear      (501) staff       (20)      885 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/entity/MessageBuilder.py
+-rw-r--r--   0 noear      (501) staff       (20)     2045 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/entity/MessageDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      215 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/entity/StringEntity.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/entity/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.065816 socket.d-2.4.11/socketd/transport/core/fragment/
+-rw-r--r--   0 noear      (501) staff       (20)     2179 2024-04-23 02:49:12.000000 socket.d-2.4.11/socketd/transport/core/fragment/FragmentAggregatorDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)     3377 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/fragment/FragmentHandlerBase.py
+-rw-r--r--   0 noear      (501) staff       (20)      502 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/fragment/FragmentHandlerDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      188 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/fragment/FragmentHolder.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/fragment/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.075247 socket.d-2.4.11/socketd/transport/core/impl/
+-rw-r--r--   0 noear      (501) staff       (20)     2358 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/impl/ChannelBase.py
+-rw-r--r--   0 noear      (501) staff       (20)     7305 2024-04-23 02:49:12.000000 socket.d-2.4.11/socketd/transport/core/impl/ChannelDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)     6579 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/impl/ConfigBase.py
+-rw-r--r--   0 noear      (501) staff       (20)      267 2024-04-20 12:58:36.000000 socket.d-2.4.11/socketd/transport/core/impl/LogConfig.py
+-rw-r--r--   0 noear      (501) staff       (20)     7943 2024-04-23 02:49:12.000000 socket.d-2.4.11/socketd/transport/core/impl/ProcessorDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)     1355 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/impl/SessionBase.py
+-rw-r--r--   0 noear      (501) staff       (20)     4288 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/impl/SessionDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/impl/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.092011 socket.d-2.4.11/socketd/transport/core/listener/
+-rw-r--r--   0 noear      (501) staff       (20)     2384 2024-04-23 02:49:12.000000 socket.d-2.4.11/socketd/transport/core/listener/EventListener.py
+-rw-r--r--   0 noear      (501) staff       (20)     1297 2024-04-23 02:49:12.000000 socket.d-2.4.11/socketd/transport/core/listener/PathListener.py
+-rw-r--r--   0 noear      (501) staff       (20)     1254 2024-04-23 02:49:12.000000 socket.d-2.4.11/socketd/transport/core/listener/PipelineListener.py
+-rw-r--r--   0 noear      (501) staff       (20)      406 2024-04-22 14:42:26.000000 socket.d-2.4.11/socketd/transport/core/listener/RouteSelector.py
+-rw-r--r--   0 noear      (501) staff       (20)      559 2024-04-22 17:36:14.000000 socket.d-2.4.11/socketd/transport/core/listener/RouteSelectorDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      473 2024-04-22 17:02:26.000000 socket.d-2.4.11/socketd/transport/core/listener/SimpleListener.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/core/listener/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.099231 socket.d-2.4.11/socketd/transport/server/
+-rw-r--r--   0 noear      (501) staff       (20)      642 2024-04-20 10:08:08.000000 socket.d-2.4.11/socketd/transport/server/Server.py
+-rw-r--r--   0 noear      (501) staff       (20)     2629 2024-04-23 02:50:04.000000 socket.d-2.4.11/socketd/transport/server/ServerBase.py
+-rw-r--r--   0 noear      (501) staff       (20)     1652 2024-04-20 10:46:19.000000 socket.d-2.4.11/socketd/transport/server/ServerConfig.py
+-rw-r--r--   0 noear      (501) staff       (20)      250 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/server/ServerProvider.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/server/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.105740 socket.d-2.4.11/socketd/transport/stream/
+-rw-r--r--   0 noear      (501) staff       (20)     1355 2024-04-23 02:48:32.000000 socket.d-2.4.11/socketd/transport/stream/RequestStream.py
+-rw-r--r--   0 noear      (501) staff       (20)      332 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/stream/SendStream.py
+-rw-r--r--   0 noear      (501) staff       (20)      690 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/stream/Stream.py
+-rw-r--r--   0 noear      (501) staff       (20)     2100 2024-04-23 02:48:32.000000 socket.d-2.4.11/socketd/transport/stream/StreamBase.py
+-rw-r--r--   0 noear      (501) staff       (20)      907 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/stream/StreamManger.py
+-rw-r--r--   0 noear      (501) staff       (20)     1025 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/stream/StreamMangerDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      843 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/stream/SubscribeStream.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/stream/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.108488 socket.d-2.4.11/socketd/transport/utils/
+-rw-r--r--   0 noear      (501) staff       (20)     3492 2024-04-19 01:32:01.000000 socket.d-2.4.11/socketd/transport/utils/AsyncUtils.py
+-rw-r--r--   0 noear      (501) staff       (20)     1989 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/utils/CompletableFuture.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/utils/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.109486 socket.d-2.4.11/socketd/transport/utils/async_api/
+-rw-r--r--   0 noear      (501) staff       (20)      787 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/utils/async_api/AtomicRefer.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/utils/async_api/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.110376 socket.d-2.4.11/socketd/transport/utils/sync_api/
+-rw-r--r--   0 noear      (501) staff       (20)      747 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/utils/sync_api/AtomicRefer.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd/transport/utils/sync_api/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.112834 socket.d-2.4.11/socketd/utils/
+-rw-r--r--   0 noear      (501) staff       (20)      216 2024-04-23 02:24:24.000000 socket.d-2.4.11/socketd/utils/RunUtils.py
+-rw-r--r--   0 noear      (501) staff       (20)      665 2024-04-19 01:32:01.000000 socket.d-2.4.11/socketd/utils/StrUtils.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-23 02:48:51.000000 socket.d-2.4.11/socketd/utils/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.134703 socket.d-2.4.11/socketd_aio_tcp/
+-rw-r--r--   0 noear      (501) staff       (20)     4143 2024-04-23 02:48:32.000000 socket.d-2.4.11/socketd_aio_tcp/TCPAIOServer.py
+-rw-r--r--   0 noear      (501) staff       (20)      517 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd_aio_tcp/TCPStreamIO.py
+-rw-r--r--   0 noear      (501) staff       (20)     2331 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd_aio_tcp/TcpAIOChannelAssistant.py
+-rw-r--r--   0 noear      (501) staff       (20)      645 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd_aio_tcp/TcpAioClient.py
+-rw-r--r--   0 noear      (501) staff       (20)     6597 2024-04-23 02:48:32.000000 socket.d-2.4.11/socketd_aio_tcp/TcpAioClientConnector.py
+-rw-r--r--   0 noear      (501) staff       (20)      776 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd_aio_tcp/TcpAioProvider.py
+-rw-r--r--   0 noear      (501) staff       (20)      183 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd_aio_tcp/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.150803 socket.d-2.4.11/socketd_websocket/
+-rw-r--r--   0 noear      (501) staff       (20)     2471 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd_websocket/WsAioChannelAssistant.py
+-rw-r--r--   0 noear      (501) staff       (20)      574 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd_websocket/WsAioClient.py
+-rw-r--r--   0 noear      (501) staff       (20)     3639 2024-04-23 02:48:32.000000 socket.d-2.4.11/socketd_websocket/WsAioClientConnector.py
+-rw-r--r--   0 noear      (501) staff       (20)      830 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd_websocket/WsAioProvider.py
+-rw-r--r--   0 noear      (501) staff       (20)     2099 2024-04-22 09:42:19.000000 socket.d-2.4.11/socketd_websocket/WsAioServer.py
+-rw-r--r--   0 noear      (501) staff       (20)      117 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd_websocket/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-23 02:53:54.156817 socket.d-2.4.11/socketd_websocket/impl/
+-rw-r--r--   0 noear      (501) staff       (20)     4784 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd_websocket/impl/AIOConnect.py
+-rw-r--r--   0 noear      (501) staff       (20)     6180 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd_websocket/impl/AIOServe.py
+-rw-r--r--   0 noear      (501) staff       (20)     5990 2024-04-23 02:48:32.000000 socket.d-2.4.11/socketd_websocket/impl/AIOWebSocketClientImpl.py
+-rw-r--r--   0 noear      (501) staff       (20)     4297 2024-04-23 02:24:50.000000 socket.d-2.4.11/socketd_websocket/impl/AIOWebSocketServerImpl.py
+-rw-r--r--   0 noear      (501) staff       (20)      274 2024-04-18 02:59:52.000000 socket.d-2.4.11/socketd_websocket/impl/__init__.py
```

### Comparing `socket.d-2.4.10.7/PKG-INFO` & `socket.d-2.4.11/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socket.d
-Version: 2.4.10.7
+Version: 2.4.11
 Summary: @noear/socket.d python project
 Home-page: https://socketd.noear.org/
 Author: noear,bai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Operating System :: OS Independent
```

### Comparing `socket.d-2.4.10.7/README.md` & `socket.d-2.4.11/README.md`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/setup.py` & `socket.d-2.4.11/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*_
 from setuptools import setup,find_packages
 
 setup(
     name='socket.d',
-    version='2.4.10.7',
+    version='2.4.11',
     description='@noear/socket.d python project',
     author='noear,bai',
     url='https://socketd.noear.org/',
     packages=find_packages(exclude=['*test*']),   # 包内不需要引用的文件夹
     install_requires=[                          # 依赖包
         'loguru',
         'websockets'
```

### Comparing `socket.d-2.4.10.7/socket.d.egg-info/PKG-INFO` & `socket.d-2.4.11/socket.d.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socket.d
-Version: 2.4.10.7
+Version: 2.4.11
 Summary: @noear/socket.d python project
 Home-page: https://socketd.noear.org/
 Author: noear,bai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Operating System :: OS Independent
```

### Comparing `socket.d-2.4.10.7/socket.d.egg-info/SOURCES.txt` & `socket.d-2.4.11/socket.d.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -76,16 +76,17 @@
 socketd/transport/core/impl/LogConfig.py
 socketd/transport/core/impl/ProcessorDefault.py
 socketd/transport/core/impl/SessionBase.py
 socketd/transport/core/impl/SessionDefault.py
 socketd/transport/core/impl/__init__.py
 socketd/transport/core/listener/EventListener.py
 socketd/transport/core/listener/PathListener.py
-socketd/transport/core/listener/PathMapper.py
 socketd/transport/core/listener/PipelineListener.py
+socketd/transport/core/listener/RouteSelector.py
+socketd/transport/core/listener/RouteSelectorDefault.py
 socketd/transport/core/listener/SimpleListener.py
 socketd/transport/core/listener/__init__.py
 socketd/transport/server/Server.py
 socketd/transport/server/ServerBase.py
 socketd/transport/server/ServerConfig.py
 socketd/transport/server/ServerProvider.py
 socketd/transport/server/__init__.py
@@ -95,20 +96,22 @@
 socketd/transport/stream/StreamBase.py
 socketd/transport/stream/StreamManger.py
 socketd/transport/stream/StreamMangerDefault.py
 socketd/transport/stream/SubscribeStream.py
 socketd/transport/stream/__init__.py
 socketd/transport/utils/AsyncUtils.py
 socketd/transport/utils/CompletableFuture.py
-socketd/transport/utils/StrUtils.py
 socketd/transport/utils/__init__.py
 socketd/transport/utils/async_api/AtomicRefer.py
 socketd/transport/utils/async_api/__init__.py
 socketd/transport/utils/sync_api/AtomicRefer.py
 socketd/transport/utils/sync_api/__init__.py
+socketd/utils/RunUtils.py
+socketd/utils/StrUtils.py
+socketd/utils/__init__.py
 socketd_aio_tcp/TCPAIOServer.py
 socketd_aio_tcp/TCPStreamIO.py
 socketd_aio_tcp/TcpAIOChannelAssistant.py
 socketd_aio_tcp/TcpAioClient.py
 socketd_aio_tcp/TcpAioClientConnector.py
 socketd_aio_tcp/TcpAioProvider.py
 socketd_aio_tcp/__init__.py
```

### Comparing `socket.d-2.4.10.7/socketd/SocketD.py` & `socket.d-2.4.11/socketd/SocketD.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from socketd.transport.server.ServerProvider import ServerProvider
 
 from socketd_websocket.WsAioProvider import WsAioProvider
 from socketd_aio_tcp.TcpAioProvider import TcpAioProvider
 
 
 def version() -> str:
-    return "2.4.10"
+    return "2.4.11"
 
 
 def protocol_version() -> str:
     return "1.0"
 
 
 client_factory_map: Dict[str, ClientProvider] = {}
```

### Comparing `socket.d-2.4.10.7/socketd/broker/BrokerListener.py` & `socket.d-2.4.11/socketd/broker/BrokerListener.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd/broker/BrokerListenerBase.py` & `socket.d-2.4.11/socketd/broker/BrokerListenerBase.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Dict, List
 from socketd.cluster.LoadBalancer import LoadBalancer
 from socketd.transport.client.ClientSession import ClientSession
 from socketd.transport.core.EntityMetas import EntityMetas
 from socketd.transport.core.Listener import Listener
 from socketd.transport.core.Message import Message
 from socketd.transport.core.Session import Session
-from socketd.transport.utils.StrUtils import StrUtils
+from socketd.utils.StrUtils import StrUtils
 
 
 # 经纪人监听器基类（实现玩家封闭管理）
 class BrokerListenerBase(Listener, ABC):
     def __init__(self):
         self.__sessionAll: Dict[str, Session] = {}
         self.__playerSessions: Dict[str, List[Session]] = {}
```

### Comparing `socket.d-2.4.10.7/socketd/cluster/ClusterClient.py` & `socket.d-2.4.11/socketd/cluster/ClusterClient.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd/cluster/ClusterClientSession.py` & `socket.d-2.4.11/socketd/cluster/ClusterClientSession.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from socketd.cluster.LoadBalancer import LoadBalancer
 from socketd.exception.SocketDExecption import SocketDException
 from socketd.transport.client.ClientSession import ClientSession
 from socketd.transport.core import Entity
 from socketd.transport.stream.RequestStream import RequestStream
 from socketd.transport.stream.SendStream import SendStream
 from socketd.transport.stream.SubscribeStream import SubscribeStream
-from socketd.transport.utils.StrUtils import StrUtils
+from socketd.utils.StrUtils import StrUtils
 
 
 class ClusterClientSession(ClientSession):
 
     def __init__(self, _sessionSet):
         self.__sessionSet: list[ClientSession] = _sessionSet
         self.__sessionId = StrUtils.guid()
```

### Comparing `socket.d-2.4.10.7/socketd/cluster/LoadBalancer.py` & `socket.d-2.4.11/socketd/cluster/LoadBalancer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from threading import RLock
 from typing import List
 
 from socketd.transport.client.ClientSession import ClientSession
-from socketd.transport.utils.StrUtils import StrUtils
+from socketd.utils.StrUtils import StrUtils
 
 
 class LoadBalancer:
     __roundCounter: int = 0  # 轮环计数器
     __lock: RLock = RLock()  # 计数锁
 
     @staticmethod
```

### Comparing `socket.d-2.4.10.7/socketd/exception/SocketDExecption.py` & `socket.d-2.4.11/socketd/exception/SocketDExecption.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd/transport/client/Client.py` & `socket.d-2.4.11/socketd/transport/client/Client.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd/transport/client/ClientBase.py` & `socket.d-2.4.11/socketd/transport/client/ClientBase.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd/transport/client/ClientChannel.py` & `socket.d-2.4.11/socketd/transport/client/ClientChannel.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd/transport/client/ClientConfig.py` & `socket.d-2.4.11/socketd/transport/client/ClientConfig.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd/transport/client/ClientSession.py` & `socket.d-2.4.11/socketd/transport/client/ClientSession.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd/transport/core/Asserts.py` & `socket.d-2.4.11/socketd/transport/core/Asserts.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd/transport/core/Channel.py` & `socket.d-2.4.11/socketd/transport/core/Channel.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd/transport/core/ChannelAssistant.py` & `socket.d-2.4.11/socketd/transport/core/ChannelAssistant.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd/transport/core/ChannelInternal.py` & `socket.d-2.4.11/socketd/transport/core/ChannelInternal.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd/transport/core/ChannelSupporter.py` & `socket.d-2.4.11/socketd/transport/core/ChannelSupporter.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd/transport/core/Codec.py` & `socket.d-2.4.11/socketd/transport/core/Codec.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,17 @@
     @abstractmethod
     def put_bytes(self, _bytes: bytearray | memoryview | bytes): ...
 
     @abstractmethod
     def put_int(self, _num: int): ...
 
     @abstractmethod
+    def put_char(self, _char: int): ...
+
+    @abstractmethod
     def flush(self): ...
 
     @abstractmethod
     def close(self): ...
 
     @abstractmethod
     def get_buffer(self) -> BytesIO: ...
```

### Comparing `socket.d-2.4.10.7/socketd/transport/core/Config.py` & `socket.d-2.4.11/socketd/transport/core/Config.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd/transport/core/Costants.py` & `socket.d-2.4.11/socketd/transport/core/Costants.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd/transport/core/Entity.py` & `socket.d-2.4.11/socketd/transport/core/Entity.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd/transport/core/EntityMetas.py` & `socket.d-2.4.11/socketd/transport/core/EntityMetas.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd/transport/core/Flags.py` & `socket.d-2.4.11/socketd/transport/core/Flags.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd/transport/core/FragmentAggregator.py` & `socket.d-2.4.11/socketd/transport/core/FragmentAggregator.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd/transport/core/FragmentHandler.py` & `socket.d-2.4.11/socketd/transport/core/FragmentHandler.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd/transport/core/Frames.py` & `socket.d-2.4.11/socketd/transport/core/Frames.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd/transport/core/HandshakeDefault.py` & `socket.d-2.4.11/socketd/transport/core/HandshakeDefault.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Dict
 from urllib.parse import urlparse, parse_qsl
 
 from socketd.transport.core.EntityMetas import EntityMetas
 from socketd.transport.core.Message import Message, MessageInternal
-from socketd.transport.utils.StrUtils import StrUtils
+from socketd.utils.StrUtils import StrUtils
 
 
 class Handshake:
     def version(self)->str:
         ...
     def uri(self):
         ...
```

### Comparing `socket.d-2.4.10.7/socketd/transport/core/Message.py` & `socket.d-2.4.11/socketd/transport/core/Message.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd/transport/core/Processor.py` & `socket.d-2.4.11/socketd/transport/core/Processor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from abc import ABC, abstractmethod
 
+from socketd.transport.core import Listener
 from socketd.transport.core.Channel import Channel
 from socketd.transport.core.ChannelInternal import ChannelInternal
 from socketd.transport.core.Frame import Frame
 from socketd.transport.core.Message import Message
 
 
 class Processor(ABC):
 
     @abstractmethod
-    def set_listener(self, listener):
+    def set_listener(self, listener: Listener) -> None:
         pass
 
     @abstractmethod
     def on_receive(self, channel: Channel, frame:Frame):
         pass
 
     @abstractmethod
@@ -27,7 +28,10 @@
     @abstractmethod
     def on_close(self, channel: ChannelInternal):
         pass
 
     @abstractmethod
     def on_error(self, channel: ChannelInternal, error):
         pass
+    @abstractmethod
+    def do_close_notice(self, channel: ChannelInternal):
+        pass
```

### Comparing `socket.d-2.4.10.7/socketd/transport/core/Session.py` & `socket.d-2.4.11/socketd/transport/core/Session.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd/transport/core/codec/Buffer.py` & `socket.d-2.4.11/socketd/transport/core/codec/Buffer.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,24 +17,31 @@
 
     def remaining(self) -> int:
         if self.__size == 0:
             self.__size = len(super().getvalue())
         rem = self.__size - self.tell()
         return rem if rem > 0 else 0
 
-    def limit(self):
-        return self.__limit
+    def position(self) -> int:
+        ...
 
     def size(self):
         return self.__size
 
+    def limit(self):
+        return self.__limit
+
     def put_int(self, num: int):
         super().write(num.to_bytes(length=4, byteorder='big', signed=False))
         self.__size += 4
 
+    def put_char(self, char:int):
+        super().write(char.to_bytes(length=2, byteorder='big', signed=False))
+        self.__size += 2
+
     def get_int(self):
         return int.from_bytes(self.read1(4), byteorder='big', signed=False)
 
     def write(self, __buffer) -> int:
         num = super().write(__buffer)
         self.__size += num
         return num
```

### Comparing `socket.d-2.4.10.7/socketd/transport/core/codec/ByteBufferCodecReader.py` & `socket.d-2.4.11/socketd/transport/core/codec/ByteBufferCodecWriter.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,27 @@
 from io import BytesIO
 
 from socketd.transport.core.codec.Buffer import Buffer
-from socketd.transport.core.Codec import CodecReader
+from socketd.transport.core.Codec import CodecWriter
 
-
-class ByteBufferCodecReader(CodecReader):
+class ByteBufferCodecWriter(CodecWriter):
 
     def __init__(self, buffer: Buffer):
         self.__buffer = buffer
 
-    def get_bytes(self) -> bytes:
-        return self.__buffer.getvalue()
-
-    def get_int(self) -> int:
-        return int.from_bytes(self.__buffer.read1(4), byteorder='little', signed=False)
+    def put_bytes(self, _bytes: bytearray | memoryview | bytes):
+        self.__buffer.write(_bytes)
 
-    def skip_bytes(self, size):
-        self.__buffer.seek(self.__buffer.tell() + size)
+    def put_int(self, _num: int):
+        self.__buffer.put_int(_num)
 
-    def remaining(self):
-        return self.__buffer.remaining()
+    def put_char(self, _char: int):
+        self.__buffer.put_char(_char)
 
-    def position(self):
-        return self.__buffer.tell()
+    def flush(self):
+        self.__buffer.flush()
 
     def get_buffer(self) -> BytesIO:
         return self.__buffer
 
     def close(self):
         self.__buffer.close()
-
-
```

### Comparing `socket.d-2.4.10.7/socketd/transport/core/codec/ByteBufferCodecWriter.py` & `socket.d-2.4.11/socketd/transport/core/codec/ByteBufferCodecReader.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 from io import BytesIO
 
 from socketd.transport.core.codec.Buffer import Buffer
-from socketd.transport.core.Codec import CodecWriter
+from socketd.transport.core.Codec import CodecReader
 
-class ByteBufferCodecWriter(CodecWriter):
+
+class ByteBufferCodecReader(CodecReader):
 
     def __init__(self, buffer: Buffer):
         self.__buffer = buffer
 
-    def put_bytes(self, _bytes: bytearray | memoryview | bytes):
-        self.__buffer.write(_bytes)
+    def get_bytes(self) -> bytes:
+        return self.__buffer.getvalue()
+
+    def get_int(self) -> int:
+        return int.from_bytes(self.__buffer.read1(4), byteorder='big', signed=False)
+
+    def skip_bytes(self, size):
+        self.__buffer.seek(self.__buffer.tell() + size)
 
-    def put_int(self, _num: int):
-        self.__buffer.write(_num.to_bytes(length=4, byteorder='little', signed=False))
+    def remaining(self):
+        return self.__buffer.remaining()
 
-    def flush(self):
-        self.__buffer.flush()
+    def position(self):
+        return self.__buffer.tell()
 
     def get_buffer(self) -> BytesIO:
         return self.__buffer
 
     def close(self):
         self.__buffer.close()
+
+
```

### Comparing `socket.d-2.4.10.7/socketd/transport/core/codec/CodecDefault.py` & `socket.d-2.4.11/socketd/transport/core/codec/CodecDefault.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,66 +51,74 @@
             target.put_int(len1)
 
             # flag
             target.put_int(frame.flag())
 
             # sid
             target.put_bytes(sidB)
-            target.put_bytes(b'\n')
+            target.put_char(10) #'\n'
 
             # event
             target.put_bytes(event)
-            target.put_bytes(b'\n')
+            target.put_char(10)
 
             # metaString
             target.put_bytes(metaStringB)
-            target.put_bytes(b'\n')
+            target.put_char(10)
 
             # _data
             if frame.message().entity().data() is not None:
                 target.put_bytes(frame.message().entity().data().getvalue())
             target.flush()
 
             return target
 
     def read(self, _reader: CodecReader) -> Frame | None:
-        len0 = _reader.get_int()
+        frameSize = _reader.get_int()
 
-        if len0 > (_reader.remaining() + 4):
+        if frameSize > (_reader.remaining() + 4):
             return None
 
         flag = _reader.get_int()  # 取前一位数据
 
-        if len0 == 8:
+        if frameSize == 8:
             # len + flag
             return Frame(Flags.of(flag), None)
         else:
             metaBufSize = min(Constants.MAX_SIZE_META_STRING, _reader.remaining())
+
             # 1. decode sid and event
-            by = Buffer(limit=metaBufSize)
-            sid = self.decodeString(_reader, by, Constants.MAX_SIZE_SID)
-            event = self.decodeString(_reader, by, Constants.MAX_SIZE_EVENT)
-            metaString = self.decodeString(_reader, by, Constants.MAX_SIZE_META_STRING)
+            buf = Buffer(limit=metaBufSize)
+
+            sid = self.decodeString(_reader, buf, Constants.MAX_SIZE_SID)
+
+            event = self.decodeString(_reader, buf, Constants.MAX_SIZE_EVENT)
+
+            metaString = self.decodeString(_reader, buf, Constants.MAX_SIZE_META_STRING)
+
             # 2. decode body
-            dataRealSize = len0 - _reader.position()
+            dataRealSize = frameSize - _reader.position()
             data: Optional[bytearray] = None
             if dataRealSize > Constants.MAX_SIZE_DATA:
                 # exceeded the limit, read and discard the bytes
                 data = bytearray(Constants.MAX_SIZE_DATA)
                 _reader.get_buffer().readinto(data)
                 for i in range(dataRealSize - Constants.MAX_SIZE_DATA):
                     _reader.get_buffer().read()
             else:
                 data = bytearray(_reader.get_buffer().read(dataRealSize))
 
-            message = MessageBuilder().flag(Flags.of(flag)).sid(sid).event(event).entity(
-                EntityDefault().meta_string_set(metaString).data_set(data)
-            ).build()
-            by.close()
+            message = (MessageBuilder()
+                       .flag(Flags.of(flag))
+                       .sid(sid)
+                       .event(event)
+                       .entity(EntityDefault().data_set(data).meta_string_set(metaString))
+                       .build())
+            buf.close()
             _reader.close()
             return Frame(message.flag(), message)
 
     def decodeString(self, reader: CodecReader, buf: Buffer, maxLen: int) -> str:
-        b = bytearray(reader.get_buffer().readline(maxLen).replace(b'\n', b''))
+        b = bytearray(reader.get_buffer().readline(maxLen).replace(b'\x00\n', b''))
         if buf.limit() < 1:
             return ""
         return b.decode(self.config.get_charset())
```

### Comparing `socket.d-2.4.10.7/socketd/transport/core/entity/EntityDefault.py` & `socket.d-2.4.11/socketd/transport/core/entity/EntityDefault.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd/transport/core/entity/FileEntity.py` & `socket.d-2.4.11/socketd/transport/core/entity/FileEntity.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd/transport/core/entity/MessageBuilder.py` & `socket.d-2.4.11/socketd/transport/core/entity/MessageBuilder.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd/transport/core/entity/MessageDefault.py` & `socket.d-2.4.11/socketd/transport/core/entity/MessageDefault.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd/transport/core/fragment/FragmentAggregatorDefault.py` & `socket.d-2.4.11/socketd/transport/core/fragment/FragmentAggregatorDefault.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from socketd.transport.core.Message import MessageInternal
 from socketd.transport.core.EntityMetas import EntityMetas
 from socketd.transport.core.FragmentAggregator import FragmentAggregator
 from socketd.exception.SocketDExecption import SocketDException
 
 from .FragmentHolder import FragmentHolder
 from ..entity.MessageBuilder import MessageBuilder
-from ...utils.StrUtils import StrUtils
+from socketd.utils.StrUtils import StrUtils
 
 
 class FragmentAggregatorDefault(FragmentAggregator):
     """
     分片聚合器
     """
 
@@ -39,18 +39,22 @@
 
     def get_data_stream_size(self) -> int:
         return self.__data_stream_size
 
     def get(self) -> Frame:
         self.__fragmentHolders.sort(key=lambda x: x.index)
 
-        byte: BytesIO = BytesIO()
+        dataBuffer: BytesIO = BytesIO()
 
         for fragment in self.__fragmentHolders:
-            byte.write(fragment.message.data().getvalue())
+            dataBuffer.write(fragment.message.data().getvalue())
+
+        entity = EntityDefault().meta_map_put(self.__main.meta_map()).data_set(dataBuffer)
+        entity.meta_map().pop(EntityMetas.META_DATA_FRAGMENT_IDX)
 
         return Frame(self.__main.flag(),
                      MessageBuilder()
                      .flag(self.__main.flag())
                      .sid(self.__main.sid())
-                     .entity(EntityDefault().meta_map_put(self.__main.entity().meta_map())).build()
-                     )
+                     .event(self.__main.event())
+                     .entity(entity)
+                     .build())
```

### Comparing `socket.d-2.4.10.7/socketd/transport/core/fragment/FragmentHandlerBase.py` & `socket.d-2.4.11/socketd/transport/core/fragment/FragmentHandlerBase.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd/transport/core/impl/ChannelBase.py` & `socket.d-2.4.11/socketd/transport/core/impl/ChannelBase.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd/transport/core/impl/ChannelDefault.py` & `socket.d-2.4.11/socketd/transport/core/impl/ChannelDefault.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from socketd.transport.core.Costants import Constants
 from socketd.transport.core.Flags import Flags
 from socketd.transport.core.EntityMetas import EntityMetas
 from socketd.transport.core.Session import Session
 from socketd.transport.core.impl.SessionDefault import SessionDefault
 from socketd.transport.core.Frame import Frame
 from socketd.transport.utils.CompletableFuture import CompletableFuture
+from socketd.utils.RunUtils import RunUtils
 
 S = TypeVar("S")
 
 
 class ChannelDefault(ChannelBase, ChannelInternal):
 
     def __init__(self, source: S, supporter: ChannelSupporter[S]):
@@ -34,14 +35,15 @@
         self._processor = supporter.get_processor()
         self._assistant = supporter.get_assistant()
         self._streamManger: StreamManger = supporter.get_config().get_stream_manger()
 
         self._session: Optional[Session] = None
         self._liveTime: Optional[float] = None
         self._closeCode: int = 0
+        self._isCloseNotified = False;
 
     def is_valid(self) -> bool:
         return self.is_closed() == 0 and self._assistant.is_valid(self._source)
 
     def is_closing(self) -> bool:
         return self._closeCode == Constants.CLOSE1000_PROTOCOL_CLOSE_STARTING
 
@@ -156,17 +158,27 @@
             self.onOpenFuture.cancel()
             self.onOpenFuture.set_e(e)
 
     async def close(self, code):
         try:
             self._closeCode = code
 
-            await super().close(code)
+            await RunUtils.waitTry(super().close(code))
 
             if code > Constants.CLOSE1000_PROTOCOL_CLOSE_STARTING:
                 if self._assistant.is_valid(self._source):
                     # 如果有效且非预关闭，则尝试关闭源
-                    await self._assistant.close(self._source)
+                    await RunUtils.waitTry(self._assistant.close(self._source))
                     log.debug(f"{self.get_config().get_role_name()} channel closed, sessionId={self.get_session().session_id()}")
         except Exception as e:
             log.warning(f"{self.get_config().get_role_name()} channel close error, "
                         f"sessionId={self.get_session().session_id()} : {e}")
+
+        if code > Constants.CLOSE1000_PROTOCOL_CLOSE_STARTING:
+            self.on_close_do()
+
+
+    def on_close_do(self):
+        if self._isCloseNotified == False:
+            self._isCloseNotified = True
+            self._processor.do_close_notice(self)
+
```

### Comparing `socket.d-2.4.10.7/socketd/transport/core/impl/ConfigBase.py` & `socket.d-2.4.11/socketd/transport/core/impl/ConfigBase.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd/transport/core/impl/ProcessorDefault.py` & `socket.d-2.4.11/socketd/transport/core/impl/ProcessorDefault.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import asyncio
 from abc import ABC
 from typing import Optional
 
 from socketd.exception.SocketDExecption import SocketDAlarmException, SocketDConnectionException
 from socketd.transport.core.ChannelInternal import ChannelInternal
 from socketd.transport.core.HandshakeDefault import HandshakeDefault
 from socketd.transport.core.Message import Message
@@ -10,14 +9,15 @@
 from socketd.transport.core.Costants import Constants
 from socketd.transport.core.Flags import Flags
 from socketd.transport.core.EntityMetas import EntityMetas
 from socketd.transport.core.Frame import Frame
 from socketd.transport.core.impl.LogConfig import log
 from socketd.transport.core.listener.SimpleListener import SimpleListener
 from socketd.transport.stream.StreamManger import StreamInternal
+from socketd.utils.RunUtils import RunUtils
 
 
 class ProcessorDefault(Processor, ABC):
 
     def __init__(self):
         self.listener = SimpleListener()
 
@@ -139,39 +139,45 @@
             if stream:
                 stream.on_progress(False, streamIndex, streamTotal)
             await channel.retrieve(frame, stream)
         else:
             self.on_message(channel, frame.message())
 
     def on_open(self, channel: ChannelInternal):
-        asyncio.create_task(self.on_open_do(channel))
+        RunUtils.taskTry(self.on_open_do(channel))
 
     async def on_open_do(self, channel: ChannelInternal):
         try:
             await self.listener.on_open(channel.get_session())
             channel.do_open_future(True, None)
         except Exception as e:
             log.warning("{} channel listener onOpen error", channel.get_config().get_role_name(), e)
             channel.do_open_future(False, e)
 
     def on_message(self, channel: ChannelInternal, message: Message):
-        asyncio.create_task(self.on_message_do(channel, message))
+        RunUtils.taskTry(self.on_message_do(channel, message))
 
     async def on_message_do(self, channel: ChannelInternal, message: Message):
         try:
             await self.listener.on_message(channel.get_session(), message)
         except Exception as e:
             log.warning("{} channel listener onMessage error", channel.get_config().get_role_name(), e)
             self.on_error(channel, e)
 
     def on_close(self, channel: ChannelInternal):
         if channel.is_closed() <= Constants.CLOSE1000_PROTOCOL_CLOSE_STARTING:
-            asyncio.create_task(self.on_close_internal(channel, Constants.CLOSE2003_DISCONNECTION))
+            RunUtils.taskTry(self.on_close_internal(channel, Constants.CLOSE2003_DISCONNECTION))
 
     async def on_close_internal(self, channel: ChannelInternal, code: int):
         await channel.close(code)
 
-        if code > Constants.CLOSE1000_PROTOCOL_CLOSE_STARTING:
-            await self.listener.on_close(channel.get_session())
-
     def on_error(self, channel: ChannelInternal, error):
-        self.listener.on_error(channel.get_session(), error)
+        RunUtils.taskTry(self.listener.on_error(channel.get_session(), error))
+
+    def do_close_notice(self, channel: ChannelInternal):
+         RunUtils.taskTry(self.do_close_notice_internal(channel))
+
+    async def do_close_notice_internal(self, channel: ChannelInternal):
+        try:
+            await RunUtils.waitTry(self.listener.on_close(channel.get_session()))
+        except Exception as e:
+            self.on_error(channel, e)
```

### Comparing `socket.d-2.4.10.7/socketd/transport/core/impl/SessionBase.py` & `socket.d-2.4.11/socketd/transport/core/impl/SessionBase.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd/transport/core/impl/SessionDefault.py` & `socket.d-2.4.11/socketd/transport/core/impl/SessionDefault.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd/transport/core/listener/EventListener.py` & `socket.d-2.4.11/socketd/transport/core/listener/EventListener.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,57 +1,59 @@
-from typing import Callable, Union, Dict
+from typing import Callable, Union, Dict, Coroutine
 
 from socketd.transport.core.Listener import Listener
 from socketd.transport.core.Session import Session
 from socketd.transport.core.Message import Message
+from socketd.utils.RunUtils import RunUtils
 
 
 class EventListener(Listener):
     """
     @author bai
     @since 2.0
     """
 
     def __init__(self):
-        self._doOnOpenHandler: Union[Callable[[Session], None], None] = None
-        self._doOnMessageHandler: Union[Callable[[Session, Message], None], None] = None
-        self._doOnCloseHandler: Union[Callable[[Session], None], None] = None
-        self._doOnErrorHandler: Union[Callable[[Session, Exception], None], None] = None
-        self._eventRouteSelector: Union[Dict[str, Callable[[Session, Message], None]], None] = None
+        self._doOnOpenHandler: Union[Callable[[Session], Coroutine], None] = None
+        self._doOnMessageHandler: Union[Callable[[Session, Message], Coroutine], None] = None
+        self._doOnCloseHandler: Union[Callable[[Session], Coroutine], None] = None
+        self._doOnErrorHandler: Union[Callable[[Session, Exception], Coroutine], None] = None
+        self._eventRouteSelector: Dict[str, Callable[[Session, Message], Coroutine]] = {}
 
-    def do_on_open(self, _on_open_handler: Callable[[Session, Message], None]) -> 'EventListener':
-        self._doOnOpenHandler = _on_open_handler
+    def do_on_open(self, handler: Callable[[Session], None]) -> 'EventListener':
+        self._doOnOpenHandler = handler
         return self
 
-    def do_on_message(self, _on_message_handler: Callable[[Session], None]) -> 'EventListener':
-        self._doOnMessageHandler = _on_message_handler
+    def do_on_message(self, handler: Callable[[Session, Message], None]) -> 'EventListener':
+        self._doOnMessageHandler = handler
         return self
 
-    def do_on_close(self, _on_close_handler: Callable[[Session, Exception], None]) -> 'EventListener':
-        self._doOnCloseHandler = _on_close_handler
+    def do_on_close(self, handler: Callable[[Session], None]) -> 'EventListener':
+        self._doOnCloseHandler = handler
         return self
 
-    def do_on_error_handler(self, _on_error_handler: Callable[[Session, Exception], None]) -> 'EventListener':
-        self._doOnErrorHandler = _on_error_handler
+    def do_on_error(self, handler: Callable[[Session, Exception], None]) -> 'EventListener':
+        self._doOnErrorHandler = handler
         return self
 
-    def do_on(self, event: str, handler: Callable[[Session, Message], None]):
+    def do_on(self, event: str, handler: Callable[[Session, Message], None]) -> 'EventListener':
         self._eventRouteSelector[event] = handler
+        return self
 
     async def on_open(self, session: Session):
         if self._doOnOpenHandler:
-            self._doOnOpenHandler(session)
+            await RunUtils.waitTry(await self._doOnOpenHandler(session))
 
     async def on_message(self, session: Session, message: Message):
         if self._doOnMessageHandler:
-            self._doOnMessageHandler(session, message)
+            await RunUtils.waitTry(self._doOnMessageHandler(session, message))
 
         if message_handler := self._eventRouteSelector.get(message.event()):
-            message_handler(session, message)
+            await RunUtils.waitTry(message_handler(session, message))
 
-    def on_close(self, session: Session):
+    async def on_close(self, session: Session):
         if self._doOnCloseHandler:
-            self._doOnCloseHandler(session)
+            await RunUtils.waitTry(self._doOnCloseHandler(session))
 
-    def on_error(self, session: Session, error: Exception):
+    async def on_error(self, session: Session, error: Exception):
         if self._doOnErrorHandler:
-            self._doOnErrorHandler(session, error)
+             await RunUtils.waitTry(self._doOnErrorHandler(session, error))
```

### Comparing `socket.d-2.4.10.7/socketd/transport/core/listener/PathListener.py` & `socket.d-2.4.11/socketd/transport/core/listener/PipelineListener.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,42 @@
-from __future__ import annotations
-from typing import Dict
 
-from socketd.transport.core.Listener import Listener
+from socketd.transport.core import Listener
+from socketd.transport.core.Message import Message
 from socketd.transport.core.Session import Session
-from socketd.transport.core.listener.PathMapper import PathMapperDefault
+from socketd.utils.RunUtils import RunUtils
 
 
-class PathListener(Listener):
+class PipelineListener(Listener):
 
-    def __init__(self, mapper: PathMapperDefault):
-        self._mapper: Dict[str, Listener] | PathMapperDefault = mapper
+    def __init__(self):
+        self._deque: list[Listener] = []
 
-    def of(self, path: str, listener: Listener) -> PathListener:
-        self._mapper[path] = listener
+    def prev(self, listener: Listener) -> 'PipelineListener':
+        self._deque.insert(0, listener)
         return self
 
+    def next(self, listener: Listener) -> 'PipelineListener':
+        self._deque.append(listener)
+        return self
+
+    def size(self) -> int:
+        return self._deque.__len__()
+
     async def on_open(self, session: Session):
-        if l := self._mapper.get(session.path()):
-            await l.on_open(session)
+        for listener in self._deque:
+            await RunUtils.waitTry(listener.on_open(session))
+
+    async def on_message(self, session: Session, message: Message):
+        for listener in self._deque:
+            await RunUtils.waitTry(listener.on_message(session, message))
+
+    async def on_close(self, session: Session):
+        for listener in self._deque:
+            await RunUtils.waitTry(listener.on_close(session))
+
+    async def on_error(self, session: Session, error:Exception):
+        for listener in self._deque:
+            await RunUtils.waitTry(listener.on_error(session, error))
+
+
+
 
-    async def on_message(self, session, message):
-        if l := self._mapper.get(session.path()):
-            await l.on_message(session)
-
-    async def on_close(self, session):
-        if l := self._mapper.get(session.path()):
-            await l.on_close(session)
-
-    def on_error(self, session, error):
-        if l := self._mapper.get(session.path()):
-            l.on_error(session)
```

### Comparing `socket.d-2.4.10.7/socketd/transport/server/Server.py` & `socket.d-2.4.11/socketd/transport/server/Server.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from __future__ import annotations
 
 from typing import Callable, Coroutine
 
-from websockets.sync.server import WebSocketServer
-
 from socketd.transport.server.ServerConfig import ServerConfig
 from socketd.transport.core.Listener import Listener
 
 #服务端接口
 class Server:
     #获取台头
     def get_title(self): ...
@@ -18,14 +16,14 @@
     #配置
     def config(self, consumer: Callable[[ServerConfig], None]) -> Server: ...
 
     #监听
     def listen(self, listener: Listener) -> Server: ...
 
     #启动
-    def start(self) -> WebSocketServer | Coroutine: ...
+    async def start(self) -> Server: ...
 
     #预停止
-    def prestop(self) -> Coroutine: ...
+    async def prestop(self): ...
 
     #停止
-    def stop(self) -> Coroutine: ...
+    async def stop(self): ...
```

### Comparing `socket.d-2.4.10.7/socketd/transport/server/ServerBase.py` & `socket.d-2.4.11/socketd/transport/server/ServerBase.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from socketd.transport.core.Processor import Processor
 from socketd.transport.core.Session import Session
 from socketd.transport.core.listener.SimpleListener import SimpleListener
 from socketd.transport.server.Server import Server
 from socketd.transport.server.ServerConfig import ServerConfig
 from socketd.transport.core.impl.ProcessorDefault import ProcessorDefault
 from socketd.transport.core.ChannelAssistant import ChannelAssistant
+from socketd.utils.RunUtils import RunUtils
+
 
 class ServerBase(Server,Listener):
     """
     服务端基类
     """
 
     def __init__(self, config:ServerConfig, assistant:ChannelAssistant):
@@ -58,29 +60,32 @@
         await self.prestop_do()
 
     async def stop(self):
         await self.stop_do()
 
     async def on_open(self, s: Session):
         self._sessions.add(s)
-        await self._listener.on_open(s)
+        await RunUtils.waitTry(self._listener.on_open(s))
 
     async def on_message(self, s: Session, m: Message):
-        await self._listener.on_message(s,m)
+        await RunUtils.waitTry(self._listener.on_message(s, m))
 
     async def on_close(self, s: Session):
         self._sessions.remove(s)
-        await self._listener.on_close(s)
+        await RunUtils.waitTry(self._listener.on_close(s))
 
-    def on_error(self, s: Session, e):
-        self._listener.on_error(s)
+    async def on_error(self, s: Session, e:Exception):
+        await RunUtils.waitTry(self._listener.on_error(s, e))
 
     async def prestop_do(self):
-        for s1 in self._sessions:
+        tmp = list(self._sessions)
+        for s1 in tmp:
             if s1.is_valid():
                 await s1.preclose()
+
     async def stop_do(self):
-        for s1 in self._sessions:
+        tmp = list(self._sessions)
+        for s1 in tmp:
             if s1.is_valid():
                 await s1.close()
 
         self._sessions.clear()
```

### Comparing `socket.d-2.4.10.7/socketd/transport/server/ServerConfig.py` & `socket.d-2.4.11/socketd/transport/server/ServerConfig.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
         self.__schema = schema
 
         if schema.startswith("sd:"):
             schema = schema[3:]
 
         self.__schemaCleaned = schema;
-        self.__host = ""
+        self.__host = "0.0.0.0"
         self.__port = 8602
 
     def get_schema(self):
         return self.__schema
 
     def get_host(self) -> str:
         return self.__host
```

### Comparing `socket.d-2.4.10.7/socketd/transport/stream/RequestStream.py` & `socket.d-2.4.11/socketd/transport/stream/RequestStream.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd/transport/stream/Stream.py` & `socket.d-2.4.11/socketd/transport/stream/Stream.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd/transport/stream/StreamBase.py` & `socket.d-2.4.11/socketd/transport/stream/StreamBase.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd/transport/stream/StreamManger.py` & `socket.d-2.4.11/socketd/transport/stream/StreamManger.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd/transport/stream/StreamMangerDefault.py` & `socket.d-2.4.11/socketd/transport/stream/StreamMangerDefault.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd/transport/stream/SubscribeStream.py` & `socket.d-2.4.11/socketd/transport/stream/SubscribeStream.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd/transport/utils/AsyncUtils.py` & `socket.d-2.4.11/socketd/transport/utils/AsyncUtils.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd/transport/utils/CompletableFuture.py` & `socket.d-2.4.11/socketd/transport/utils/CompletableFuture.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd/transport/utils/StrUtils.py` & `socket.d-2.4.11/socketd/utils/StrUtils.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd/transport/utils/async_api/AtomicRefer.py` & `socket.d-2.4.11/socketd/transport/utils/async_api/AtomicRefer.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd/transport/utils/sync_api/AtomicRefer.py` & `socket.d-2.4.11/socketd/transport/utils/sync_api/AtomicRefer.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd_aio_tcp/TCPAIOServer.py` & `socket.d-2.4.11/socketd_aio_tcp/TCPAIOServer.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
                          self.get_config().get_port()))
         self._sock.settimeout(self.get_config().get_idle_timeout() / 1000)
         # 生成一个服务器
         self._server: asyncio.Server = await loop.create_server(factory,
                                                                 sock=self._sock,
                                                                 start_serving=True,
                                                                 )
-        return self._server
+        await self._server
 
     async def stop(self):
         log.info("TcpAioServer stop...")
         # 等等执行完成
         await self._is_close.set(True)
         self._server.close()
         if self._sock is not None and not getattr(self._sock, "_closed"):
```

### Comparing `socket.d-2.4.10.7/socketd_aio_tcp/TCPStreamIO.py` & `socket.d-2.4.11/socketd_aio_tcp/TCPStreamIO.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd_aio_tcp/TcpAIOChannelAssistant.py` & `socket.d-2.4.11/socketd_aio_tcp/TcpAIOChannelAssistant.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd_aio_tcp/TcpAioClient.py` & `socket.d-2.4.11/socketd_aio_tcp/TcpAioClient.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd_aio_tcp/TcpAioClientConnector.py` & `socket.d-2.4.11/socketd_aio_tcp/TcpAioClientConnector.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd_aio_tcp/TcpAioProvider.py` & `socket.d-2.4.11/socketd_aio_tcp/TcpAioProvider.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd_websocket/WsAioChannelAssistant.py` & `socket.d-2.4.11/socketd_websocket/WsAioChannelAssistant.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd_websocket/WsAioClient.py` & `socket.d-2.4.11/socketd_websocket/WsAioClient.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd_websocket/WsAioClientConnector.py` & `socket.d-2.4.11/socketd_websocket/WsAioClientConnector.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd_websocket/WsAioProvider.py` & `socket.d-2.4.11/socketd_websocket/WsAioProvider.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd_websocket/WsAioServer.py` & `socket.d-2.4.11/socketd_websocket/WsAioServer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import Optional
 
-from websockets.server import WebSocketServer, serve as Serve, WebSocketServerProtocol
-from websockets import broadcast
+from websockets.server import serve as Serve
 
 from socketd import SocketD
 from socketd.transport.core.Costants import Constants
 from socketd.transport.server.ServerBase import ServerBase
 from socketd_websocket.WsAioChannelAssistant import WsAioChannelAssistant
 from socketd.transport.server.ServerConfig import ServerConfig
 from socketd_websocket.impl.AIOServe import AIOServe
@@ -16,18 +15,21 @@
 
 class WsAioServer(ServerBase):
 
     def __init__(self, config: ServerConfig):
         super().__init__(config, WsAioChannelAssistant(config))
         self._server: Optional[Serve] = None
 
+    def __del__(self):
+        del self._server
+
     def get_title(self):
         return "ws/aio/py-websocket/v" + SocketD.version();
 
-    async def start(self) -> WebSocketServer:
+    async def start(self):
         if self._isStarted:
             raise Exception("Socket.D server started")
         else:
             self._isStarted = True
 
         __host:str
         if self.get_config().get_host() is None:
@@ -36,23 +38,22 @@
             __host = self.get_config().get_host()
 
         self._server = AIOServe(ws_handler=None,
                            host=__host,
                            port=self.get_config().get_port(),
                            create_protocol=AIOWebSocketServerImpl,
                            ws_aio_server=self,
-                           ping_interval=self.get_config().get_idle_timeout(),
-                           ping_timeout=self.get_config().get_idle_timeout(),
                            ssl=self.get_config().get_ssl_context(),
                            logger=logger,
-                           max_size=Constants.MAX_SIZE_FRAME,
+                           max_size=Constants.MAX_SIZE_FRAME
                            )
 
         log.info("Socket.D server started: {server=" + self.get_config().get_local_url() + "}")
-        return await self._server
+        await self._server
+        return self
 
     async def stop(self):
         if self._isStarted:
             self._isStarted = False
         else:
             return
```

### Comparing `socket.d-2.4.10.7/socketd_websocket/impl/AIOConnect.py` & `socket.d-2.4.11/socketd_websocket/impl/AIOConnect.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd_websocket/impl/AIOServe.py` & `socket.d-2.4.11/socketd_websocket/impl/AIOServe.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd_websocket/impl/AIOWebSocketClientImpl.py` & `socket.d-2.4.11/socketd_websocket/impl/AIOWebSocketClientImpl.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.7/socketd_websocket/impl/AIOWebSocketServerImpl.py` & `socket.d-2.4.11/socketd_websocket/impl/AIOWebSocketServerImpl.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,111 +1,107 @@
 from __future__ import annotations
 import asyncio
 from typing import Optional, Union
 
-from websockets import ConnectionClosedError, ConnectionClosedOK
+from websockets import ConnectionClosedOK
+from websockets.frames import Opcode
 from websockets.server import WebSocketServer, WebSocketServerProtocol
 
 from socketd.transport.core.Channel import Channel
+from socketd.transport.core.ChannelInternal import ChannelInternal
 from socketd.transport.core.impl.LogConfig import log
 from socketd.transport.core.impl.ChannelDefault import ChannelDefault
 from socketd.transport.core.Flags import Flags
 from socketd.transport.core.Frame import Frame
 
 
 class AIOWebSocketServerImpl(WebSocketServerProtocol):
 
     def __init__(self, ws_handler, ws_server: WebSocketServer, ws_aio_server: 'WsAioServer',
                  *args, **kwargs):
         self.ws_aio_server = ws_aio_server
         self.__ws_server: WebSocketServer = ws_server
         self.__attachment: Optional[Channel] = None
-        WebSocketServerProtocol.__init__(self=self, ws_handler=self.on_message, ws_server=self.__ws_server,
+        WebSocketServerProtocol.__init__(self=self,
+                                         ws_handler=self.on_message,
+                                         ws_server=self.__ws_server,
                                          *args,
                                          **kwargs)
 
-    def set_attachment(self, obj: Channel):
+    def set_attachment(self, obj: ChannelInternal):
         self.__attachment = obj
 
-    def get_attachment(self) -> Channel:
+    def get_attachment(self) -> ChannelInternal:
         return self.__attachment
 
     def connection_open(self) -> None:
         """握手完成回调"""
         super().connection_open()
-        log.debug("AIOWebSocketServerImpl connection_open")
         self.on_open(self)
 
-    def handshake_handler(self):
-        """socket_handshake"""
-        log.debug("handshake_handler")
+    async def read_frame(self, max_size: Optional[int]) -> Frame:
+        frame = await super().read_frame(max_size)
+        if frame is not None:
+            if frame.opcode == Opcode.PONG:
+                await self.assert_handshake()
+        return frame
 
     def on_open(self, conn) -> None:
         """create_protocol"""
         if self.get_attachment() is None:
             channel = ChannelDefault(conn, self.ws_aio_server)
             self.set_attachment(channel)
 
     async def on_error(self, conn: Union[AIOWebSocketServerImpl, WebSocketServerProtocol], ex: Exception):
         try:
-            channel: Channel = conn.get_attachment()
+            channel: ChannelInternal = conn.get_attachment()
             if channel is not None:
                 # 有可能未 onOpen，就 onError 了；此时通道未成
                 self.ws_aio_server.get_processor().on_error(channel, ex)
         except Exception as e:
-            log.error(e)
-            raise e
+            log.warning(e)
 
     async def on_message(self, conn: Union[AIOWebSocketServerImpl, WebSocketServerProtocol], path: str):
         """ws_handler"""
         loop = asyncio.get_running_loop()
         tasks: list[asyncio.Task] = []
         while True:
             if conn.closed:
                 break
             try:
                 if tasks:
                     task = tasks[0]
                     if task.done():
                         tasks.pop(0)
                 message = await self.recv()
-                # frame: Frame = self.ws_aio_server.get_assistant().read(
-                #     message)
-                # # 采用线程池执行IO耗时任务
+                # 采用线程池执行IO耗时任务
                 frame: Frame = await loop.run_in_executor(self.ws_aio_server.get_config().get_exchange_executor(),
                                                           lambda _message: self.ws_aio_server.get_assistant().read(
                                                               _message), message)
                 if frame is not None:
                     # 不等待直接运行
                     tasks.append(
                         loop.create_task(self.ws_aio_server.get_processor().on_receive(self.get_attachment(), frame)))
                     if frame.flag() == Flags.Close:
-                        """客户端主动关闭"""
-                        await self.on_close(conn)
-                        log.debug("{sessionId} 主动退出",
-                                  sessionId=conn.get_attachment().get_session().session_id())
+                        # 不需要再 while(true) 了 //其它处理在 processor
                         break
-            except asyncio.CancelledError as c:
-                log.warning(c)
+
+
+            except asyncio.CancelledError as e:
                 break
             except ConnectionClosedOK as e:
-                # received 1000 (OK); then sent 1000 (OK) 或者 1001  成功直接忽略
-                log.info(e)
-                break
-            except ConnectionClosedError as e:
-                # 客户端异常关闭
-                log.error(e)
                 break
             except Exception as e:
-                log.error(e)
                 await self.on_error(conn, e)
-        try:
-            # 等待未完成任务
-            await asyncio.wait(tasks, timeout=10)
-        except asyncio.CancelledError as c:
-            pass
-        except TimeoutError as e:
-            log.warning(f"server on_receive timeout {e}")
-
-    async def on_close(self, conn: Union[AIOWebSocketServerImpl, WebSocketServerProtocol]):
-        """关闭tcp,结束握手"""
-        await conn.close()
+
+    # 未签名前，禁止 ping/pong
+    async def assert_handshake(self) -> bool:
+        channel: ChannelInternal = self.get_attachment()
+        if channel is None or channel.get_handshake() is None:
+            try:
+                await self.close()
+            except Exception:
+                ...
+            log.warning("Server channel no handshake onPingPong")
+            return False
+        else:
+            return True
```

