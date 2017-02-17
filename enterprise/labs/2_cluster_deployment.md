```
{
  "timestamp" : "2017-02-17T04:20:13.961Z",
  "clusters" : [ {
    "name" : "Yabar",
    "version" : "CDH5",
    "services" : [ {
      "name" : "hive",
      "type" : "HIVE",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "HIVEMETASTORE",
          "items" : [ {
            "name" : "hive_metastore_java_heapsize",
            "value" : "612368384"
          } ]
        }, {
          "roleType" : "HIVESERVER2",
          "items" : [ {
            "name" : "hiveserver2_java_heapsize",
            "value" : "612368384"
          }, {
            "name" : "hiveserver2_spark_driver_memory",
            "value" : "966367641"
          }, {
            "name" : "hiveserver2_spark_executor_cores",
            "value" : "4"
          }, {
            "name" : "hiveserver2_spark_executor_memory",
            "value" : "3571397427"
          }, {
            "name" : "hiveserver2_spark_yarn_driver_memory_overhead",
            "value" : "102"
          }, {
            "name" : "hiveserver2_spark_yarn_executor_memory_overhead",
            "value" : "601"
          } ]
        } ],
        "items" : [ {
          "name" : "hive_metastore_database_host",
          "value" : "ip-172-31-0-196.ap-southeast-1.compute.internal"
        }, {
          "name" : "hive_metastore_database_name",
          "value" : "hive"
        }, {
          "name" : "hive_metastore_database_password",
          "value" : "1234"
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hive-GATEWAY-0191e269e9198a380cb54b05f867b7c2",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "c12c70f7-4f52-46f2-9085-49faf6099f69"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-a7e67f1df4d1f465460c26174e3d4071",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "4e6884af-34ae-4cfc-b64d-e12230b10b9c"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-ccf3a7808d66c03cfd6edc815fc65e2b",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "cbaaea85-dc76-4e01-8114-e640e6a859de"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-cec8c2eb5c6958fc400eb0ac2383b791",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "b0d3cf8a-0df1-41f9-b911-eb5cfa1ca177"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-GATEWAY-de04b6db4d29a905cc2111db1b3c9bfd",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "f6dc3796-0fc1-48b3-a8fd-3d6f7702f787"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-HIVEMETASTORE-de04b6db4d29a905cc2111db1b3c9bfd",
        "type" : "HIVEMETASTORE",
        "hostRef" : {
          "hostId" : "f6dc3796-0fc1-48b3-a8fd-3d6f7702f787"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "asx2llwon58jn653i4lmdhbmb"
          } ]
        }
      }, {
        "name" : "hive-HIVESERVER2-de04b6db4d29a905cc2111db1b3c9bfd",
        "type" : "HIVESERVER2",
        "hostRef" : {
          "hostId" : "f6dc3796-0fc1-48b3-a8fd-3d6f7702f787"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "b6hmtnkjqlfm4aa7yvriqckcg"
          } ]
        }
      } ],
      "displayName" : "Hive"
    }, {
      "name" : "zookeeper",
      "type" : "ZOOKEEPER",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "SERVER",
          "items" : [ {
            "name" : "zookeeper_server_java_heapsize",
            "value" : "612368384"
          } ]
        } ],
        "items" : [ ]
      },
      "roles" : [ {
        "name" : "zookeeper-SERVER-0191e269e9198a380cb54b05f867b7c2",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "c12c70f7-4f52-46f2-9085-49faf6099f69"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "8dmaq165hfw9273zpptvqw8gl"
          }, {
            "name" : "serverId",
            "value" : "3"
          } ]
        }
      }, {
        "name" : "zookeeper-SERVER-cec8c2eb5c6958fc400eb0ac2383b791",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "b0d3cf8a-0df1-41f9-b911-eb5cfa1ca177"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "1wab72ijsro394by00byseepy"
          }, {
            "name" : "serverId",
            "value" : "1"
          } ]
        }
      }, {
        "name" : "zookeeper-SERVER-de04b6db4d29a905cc2111db1b3c9bfd",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "f6dc3796-0fc1-48b3-a8fd-3d6f7702f787"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "5m25xlsh14zgs53olgrfljoq7"
          }, {
            "name" : "serverId",
            "value" : "2"
          } ]
        }
      } ],
      "displayName" : "ZooKeeper"
    }, {
      "name" : "hue",
      "type" : "HUE",
      "config" : {
        "roleTypeConfigs" : [ ],
        "items" : [ {
          "name" : "database_host",
          "value" : "ip-172-31-0-196.ap-southeast-1.compute.internal"
        }, {
          "name" : "database_password",
          "value" : "1234"
        }, {
          "name" : "database_type",
          "value" : "mysql"
        }, {
          "name" : "hive_service",
          "value" : "hive"
        }, {
          "name" : "hue_service_safety_valve",
          "value" : "[desktop]\nallowed_hosts=*"
        }, {
          "name" : "hue_webhdfs",
          "value" : "hdfs-NAMENODE-de04b6db4d29a905cc2111db1b3c9bfd"
        }, {
          "name" : "oozie_service",
          "value" : "oozie"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hue-HUE_SERVER-de04b6db4d29a905cc2111db1b3c9bfd",
        "type" : "HUE_SERVER",
        "hostRef" : {
          "hostId" : "f6dc3796-0fc1-48b3-a8fd-3d6f7702f787"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "81teat2518bm66v9lqb8bfzr0"
          }, {
            "name" : "secret_key",
            "value" : "e6PDNehMpjsk7JlxN0TVEhEBV82pg1"
          } ]
        }
      } ],
      "displayName" : "Hue"
    }, {
      "name" : "oozie",
      "type" : "OOZIE",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "OOZIE_SERVER",
          "items" : [ {
            "name" : "oozie_database_host",
            "value" : "ip-172-31-0-196.ap-southeast-1.compute.internal"
          }, {
            "name" : "oozie_database_password",
            "value" : "1234"
          }, {
            "name" : "oozie_database_type",
            "value" : "mysql"
          }, {
            "name" : "oozie_database_user",
            "value" : "oozie"
          }, {
            "name" : "oozie_java_heapsize",
            "value" : "612368384"
          } ]
        } ],
        "items" : [ {
          "name" : "hive_service",
          "value" : "hive"
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "oozie-OOZIE_SERVER-de04b6db4d29a905cc2111db1b3c9bfd",
        "type" : "OOZIE_SERVER",
        "hostRef" : {
          "hostId" : "f6dc3796-0fc1-48b3-a8fd-3d6f7702f787"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "n81fhtdl5o05t51otlybxqia"
          } ]
        }
      } ],
      "displayName" : "Oozie"
    }, {
      "name" : "yarn",
      "type" : "YARN",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "GATEWAY",
          "items" : [ {
            "name" : "mapred_reduce_tasks",
            "value" : "8"
          }, {
            "name" : "mapred_submit_replication",
            "value" : "2"
          } ]
        }, {
          "roleType" : "JOBHISTORY",
          "items" : [ {
            "name" : "mr2_jobhistory_java_heapsize",
            "value" : "612368384"
          } ]
        }, {
          "roleType" : "NODEMANAGER",
          "items" : [ {
            "name" : "yarn_nodemanager_heartbeat_interval_ms",
            "value" : "100"
          }, {
            "name" : "yarn_nodemanager_local_dirs",
            "value" : "/yarn/nm"
          }, {
            "name" : "yarn_nodemanager_log_dirs",
            "value" : "/yarn/container-logs"
          }, {
            "name" : "yarn_nodemanager_resource_cpu_vcores",
            "value" : "4"
          }, {
            "name" : "yarn_nodemanager_resource_memory_mb",
            "value" : "5250"
          } ]
        }, {
          "roleType" : "RESOURCEMANAGER",
          "items" : [ {
            "name" : "resource_manager_java_heapsize",
            "value" : "612368384"
          }, {
            "name" : "yarn_scheduler_maximum_allocation_mb",
            "value" : "5250"
          }, {
            "name" : "yarn_scheduler_maximum_allocation_vcores",
            "value" : "4"
          } ]
        } ],
        "items" : [ {
          "name" : "hdfs_service",
          "value" : "hdfs"
        }, {
          "name" : "rm_dirty",
          "value" : "true"
        }, {
          "name" : "zk_authorization_secret_key",
          "value" : "MrzDmRvFJlOdz6ZNiCnxZNRbSSE70i"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "yarn-JOBHISTORY-de04b6db4d29a905cc2111db1b3c9bfd",
        "type" : "JOBHISTORY",
        "hostRef" : {
          "hostId" : "f6dc3796-0fc1-48b3-a8fd-3d6f7702f787"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "agru4epdh12ifu3zm89vgg5md"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-0191e269e9198a380cb54b05f867b7c2",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "c12c70f7-4f52-46f2-9085-49faf6099f69"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "6yf0lsiwn8c24o661kcbtt78n"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-a7e67f1df4d1f465460c26174e3d4071",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "4e6884af-34ae-4cfc-b64d-e12230b10b9c"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "86okg5usp9z09kcn18uyyi35u"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-ccf3a7808d66c03cfd6edc815fc65e2b",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "cbaaea85-dc76-4e01-8114-e640e6a859de"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "f5830x42o27r8ozmc7m2bb0w0"
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-cec8c2eb5c6958fc400eb0ac2383b791",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "b0d3cf8a-0df1-41f9-b911-eb5cfa1ca177"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "ciams8yveippqs0i7vs73h28q"
          } ]
        }
      }, {
        "name" : "yarn-RESOURCEMANAGER-de04b6db4d29a905cc2111db1b3c9bfd",
        "type" : "RESOURCEMANAGER",
        "hostRef" : {
          "hostId" : "f6dc3796-0fc1-48b3-a8fd-3d6f7702f787"
        },
        "config" : {
          "items" : [ {
            "name" : "rm_id",
            "value" : "53"
          }, {
            "name" : "role_jceks_password",
            "value" : "264eqznjvfqbogg6y7bdv0i1y"
          } ]
        }
      } ],
      "displayName" : "YARN (MR2 Included)"
    }, {
      "name" : "hdfs",
      "type" : "HDFS",
      "config" : {
        "roleTypeConfigs" : [ {
          "roleType" : "BALANCER",
          "items" : [ {
            "name" : "balancer_java_heapsize",
            "value" : "612368384"
          } ]
        }, {
          "roleType" : "DATANODE",
          "items" : [ {
            "name" : "dfs_data_dir_list",
            "value" : "/dfs/dn"
          }, {
            "name" : "dfs_datanode_du_reserved",
            "value" : "7398261555"
          }, {
            "name" : "dfs_datanode_max_locked_memory",
            "value" : "4201644032"
          } ]
        }, {
          "roleType" : "GATEWAY",
          "items" : [ {
            "name" : "dfs_client_use_trash",
            "value" : "true"
          } ]
        }, {
          "roleType" : "NAMENODE",
          "items" : [ {
            "name" : "dfs_name_dir_list",
            "value" : "/dfs/nn"
          }, {
            "name" : "dfs_namenode_servicerpc_address",
            "value" : "8022"
          }, {
            "name" : "namenode_java_heapsize",
            "value" : "612368384"
          } ]
        }, {
          "roleType" : "SECONDARYNAMENODE",
          "items" : [ {
            "name" : "fs_checkpoint_dir_list",
            "value" : "/dfs/snn"
          }, {
            "name" : "secondary_namenode_java_heapsize",
            "value" : "612368384"
          } ]
        } ],
        "items" : [ {
          "name" : "dfs_ha_fencing_cloudera_manager_secret_key",
          "value" : "hA7bdWcqKXulnQpCLvqZMVjE6lIW9R"
        }, {
          "name" : "fc_authorization_secret_key",
          "value" : "kBOZHlRgyt1gaT4XPXphMfw2zFXs5r"
        }, {
          "name" : "http_auth_signature_secret",
          "value" : "pbjxrPclo1LBGbaRA7crztDw78siSW"
        }, {
          "name" : "rm_dirty",
          "value" : "true"
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper"
        } ]
      },
      "roles" : [ {
        "name" : "hdfs-BALANCER-de04b6db4d29a905cc2111db1b3c9bfd",
        "type" : "BALANCER",
        "hostRef" : {
          "hostId" : "f6dc3796-0fc1-48b3-a8fd-3d6f7702f787"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hdfs-DATANODE-0191e269e9198a380cb54b05f867b7c2",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "c12c70f7-4f52-46f2-9085-49faf6099f69"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "eootedwvu82777z0dl7vprrg4"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-a7e67f1df4d1f465460c26174e3d4071",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "4e6884af-34ae-4cfc-b64d-e12230b10b9c"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "bfyksefibk8y9yr0oxsdy8byb"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-ccf3a7808d66c03cfd6edc815fc65e2b",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "cbaaea85-dc76-4e01-8114-e640e6a859de"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "bde3v9tkxqvype0jkse00oe6y"
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-cec8c2eb5c6958fc400eb0ac2383b791",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "b0d3cf8a-0df1-41f9-b911-eb5cfa1ca177"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "aivtgux0b5c4lz1rsrbsjmstl"
          } ]
        }
      }, {
        "name" : "hdfs-NAMENODE-de04b6db4d29a905cc2111db1b3c9bfd",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "f6dc3796-0fc1-48b3-a8fd-3d6f7702f787"
        },
        "config" : {
          "items" : [ {
            "name" : "namenode_id",
            "value" : "55"
          }, {
            "name" : "role_jceks_password",
            "value" : "a8bnwfns939zlsjazu00gl0iy"
          } ]
        }
      }, {
        "name" : "hdfs-SECONDARYNAMENODE-de04b6db4d29a905cc2111db1b3c9bfd",
        "type" : "SECONDARYNAMENODE",
        "hostRef" : {
          "hostId" : "f6dc3796-0fc1-48b3-a8fd-3d6f7702f787"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "eospljcv6h6psmy1m07idghip"
          } ]
        }
      } ],
      "displayName" : "HDFS"
    } ]
  } ],
  "hosts" : [ {
    "hostId" : "f6dc3796-0fc1-48b3-a8fd-3d6f7702f787",
    "ipAddress" : "172.31.0.196",
    "hostname" : "ip-172-31-0-196.ap-southeast-1.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "b0d3cf8a-0df1-41f9-b911-eb5cfa1ca177",
    "ipAddress" : "172.31.11.136",
    "hostname" : "ip-172-31-11-136.ap-southeast-1.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "c12c70f7-4f52-46f2-9085-49faf6099f69",
    "ipAddress" : "172.31.12.4",
    "hostname" : "ip-172-31-12-4.ap-southeast-1.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "4e6884af-34ae-4cfc-b64d-e12230b10b9c",
    "ipAddress" : "172.31.6.40",
    "hostname" : "ip-172-31-6-40.ap-southeast-1.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "cbaaea85-dc76-4e01-8114-e640e6a859de",
    "ipAddress" : "172.31.8.210",
    "hostname" : "ip-172-31-8-210.ap-southeast-1.compute.internal",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  } ],
  "users" : [ {
    "name" : "__cloudera_internal_user__mgmt-EVENTSERVER-de04b6db4d29a905cc2111db1b3c9bfd",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "036e3c7d90dcf53db2e5e71dd41b754c9801da3a76617a647cc3627fb24d290d",
    "pwSalt" : 8741893982823738942,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-HOSTMONITOR-de04b6db4d29a905cc2111db1b3c9bfd",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "5b7ab262945257a3dc3167a4b6e9b83e051864444ad27048d1e063d497127526",
    "pwSalt" : -2154680672071633102,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-REPORTSMANAGER-de04b6db4d29a905cc2111db1b3c9bfd",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "c948a901edfd2e87c4cdd94dff48e107df362e70f864945fbb48c537c37b5ad5",
    "pwSalt" : -6667963476952581556,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-SERVICEMONITOR-de04b6db4d29a905cc2111db1b3c9bfd",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "3e24acba3731d90b80cd75741a8c72e5434c7258f61441db9d31119c146b9776",
    "pwSalt" : 8218073030938777917,
    "pwLogin" : true
  }, {
    "name" : "admin",
    "roles" : [ "ROLE_ADMIN" ],
    "pwHash" : "151cbef3a428be149cc81d9ab777089956d70d4c6c5fec29f564de48ac8f672a",
    "pwSalt" : -3559052372994049347,
    "pwLogin" : true
  } ],
  "versionInfo" : {
    "version" : "5.10.0",
    "buildUser" : "jenkins",
    "buildTimestamp" : "20170120-1038",
    "gitHash" : "aa0b5cd5eceaefe2f971c13ab657020d96bb842a",
    "snapshot" : false
  },
  "managementService" : {
    "name" : "mgmt",
    "type" : "MGMT",
    "config" : {
      "roleTypeConfigs" : [ {
        "roleType" : "EVENTSERVER",
        "items" : [ {
          "name" : "event_server_heapsize",
          "value" : "612368384"
        } ]
      }, {
        "roleType" : "HOSTMONITOR",
        "items" : [ {
          "name" : "firehose_heapsize",
          "value" : "612368384"
        }, {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "805306368"
        } ]
      }, {
        "roleType" : "REPORTSMANAGER",
        "items" : [ {
          "name" : "headlamp_database_host",
          "value" : "ip-172-31-0-196.ap-southeast-1.compute.internal"
        }, {
          "name" : "headlamp_database_name",
          "value" : "rman"
        }, {
          "name" : "headlamp_database_password",
          "value" : "1234"
        }, {
          "name" : "headlamp_database_user",
          "value" : "rman"
        }, {
          "name" : "headlamp_heapsize",
          "value" : "612368384"
        } ]
      }, {
        "roleType" : "SERVICEMONITOR",
        "items" : [ {
          "name" : "firehose_heapsize",
          "value" : "612368384"
        }, {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "805306368"
        } ]
      } ],
      "items" : [ ]
    },
    "roles" : [ {
      "name" : "mgmt-ALERTPUBLISHER-de04b6db4d29a905cc2111db1b3c9bfd",
      "type" : "ALERTPUBLISHER",
      "hostRef" : {
        "hostId" : "f6dc3796-0fc1-48b3-a8fd-3d6f7702f787"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "494evz3dkur733sys9gkpw787"
        } ]
      }
    }, {
      "name" : "mgmt-EVENTSERVER-de04b6db4d29a905cc2111db1b3c9bfd",
      "type" : "EVENTSERVER",
      "hostRef" : {
        "hostId" : "f6dc3796-0fc1-48b3-a8fd-3d6f7702f787"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "dmpjfuoe2mq5kck0iz78ojalz"
        } ]
      }
    }, {
      "name" : "mgmt-HOSTMONITOR-de04b6db4d29a905cc2111db1b3c9bfd",
      "type" : "HOSTMONITOR",
      "hostRef" : {
        "hostId" : "f6dc3796-0fc1-48b3-a8fd-3d6f7702f787"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "1343ozz3c1lapxxa2yh69qhv0"
        } ]
      }
    }, {
      "name" : "mgmt-REPORTSMANAGER-de04b6db4d29a905cc2111db1b3c9bfd",
      "type" : "REPORTSMANAGER",
      "hostRef" : {
        "hostId" : "f6dc3796-0fc1-48b3-a8fd-3d6f7702f787"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "ed8xkivyomrdrv39fbhp4yfm0"
        } ]
      }
    }, {
      "name" : "mgmt-SERVICEMONITOR-de04b6db4d29a905cc2111db1b3c9bfd",
      "type" : "SERVICEMONITOR",
      "hostRef" : {
        "hostId" : "f6dc3796-0fc1-48b3-a8fd-3d6f7702f787"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "2gfd2b93kxyddu4uosx3h0e88"
        } ]
      }
    } ],
    "displayName" : "Cloudera Management Service"
  },
  "managerSettings" : {
    "items" : [ {
      "name" : "CLUSTER_STATS_START",
      "value" : "10/24/2012 17:40"
    }, {
      "name" : "PUBLIC_CLOUD_STATUS",
      "value" : "ON_PUBLIC_CLOUD"
    }, {
      "name" : "REMOTE_PARCEL_REPO_URLS",
      "value" : "https://archive.cloudera.com/cdh5/parcels/{latest_supported}/,https://archive.cloudera.com/cdh4/parcels/latest/,https://archive.cloudera.com/impala/parcels/latest/,https://archive.cloudera.com/search/parcels/latest/,https://archive.cloudera.com/accumulo/parcels/1.4/,https://archive.cloudera.com/accumulo-c5/parcels/latest/,https://archive.cloudera.com/kafka/parcels/latest/,https://archive.cloudera.com/navigator-keytrustee5/parcels/latest/,https://archive.cloudera.com/spark/parcels/latest/,https://archive.cloudera.com/sqoop-connectors/parcels/latest/"
    } ]
  }
}
```
