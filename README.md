# 拉取静态库

```
https://github.com/RapidAI/OnnxruntimeBuilder
```

# 创建merge.mri 根据需要修改

```
create libonnxruntime.a
addlib use/libclog.a
addlib use/libcpuinfo.a
addlib use/libflatbuffers.a
addlib use/libnsync_cpp.a
addlib use/libonnx.a
addlib use/libonnx_proto.a
addlib use/libonnxruntime_common.a
addlib use/libonnxruntime_flatbuffers.a
addlib use/libonnxruntime_framework.a
addlib use/libonnxruntime_graph.a
addlib use/libonnxruntime_mlas.a
addlib use/libonnxruntime_optimizer.a
addlib use/libonnxruntime_providers.a
addlib use/libonnxruntime_session.a
addlib use/libonnxruntime_util.a
addlib use/libprotobuf-lite.a
addlib use/libre2.a
save
end
```

# 生成libonnxruntime.a

``ar -M < ./merge.mri ``
