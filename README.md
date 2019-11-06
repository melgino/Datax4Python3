# Datax4Python3 轻松让datax也能运行在python3下运行

原版的datax3是支持python2的，不过现在python已经退出历史舞台了，都是python3了，因此我们需要稍稍修改一下datax中的python文件的代码，让整个datax可以顺利地在python3下面运行（Anaconda的python也是可以的）

修改点：
##print在python2和python3的差异
例如：python2的写法
print readerRef
在python3中是
print(readerRef)

##exception在python2和python3的差异
例如：python2的写法
except Exception, e:
python3中是
except Exception as e:

就上面2类小的修改，就可以让datax3运行在python3下面了，可以将上述修改好的文件，直接覆盖自己的 datax/bin下的3个python文件即可。
