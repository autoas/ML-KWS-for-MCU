from building import *

cwd = GetCurrentDir()

Import('asenv')
MODULES = asenv['MODULES']

objs = []

objs += Glob('Deployment/Source/local_NN/*.c')
objs += Glob('Deployment/Source/NN/*/*.cpp')

asenv.Append(CPPPATH=['%s/Deployment/Source/local_NN'%(cwd),
					  '%s/Deployment/Source/NN'%(cwd),
					  '%s/Deployment/Source/NN/DNN'%(cwd),
					  '%s/Deployment/Source/NN/DS_CNN'%(cwd)])
Return('objs')

