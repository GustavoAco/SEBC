```
{
  "timestamp" : "2017-11-30T19:16:29.730Z",
  "clusters" : [ {
    "name" : "cluster",
    "displayName" : "GustavoAco",
    "version" : "CDH5",
    "fullVersion" : "5.12.1",
    "services" : [ {
      "name" : "hive",
      "type" : "HIVE",
      "config" : {
        "items" : [ {
          "name" : "hive_metastore_database_host",
          "value" : "node1.gus.com",
          "sensitive" : false
        }, {
          "name" : "hive_metastore_database_password",
          "value" : "C@paCuatro1.",
          "sensitive" : true
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn",
          "sensitive" : false
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper",
          "sensitive" : false
        } ]
      },
      "roles" : [ {
        "name" : "hive-GATEWAY-76becde789a47172e5c46b70269dfd61",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "735266e9-9647-499a-a81f-4ae2b5177969"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-GATEWAY-BASE"
        }
      }, {
        "name" : "hive-GATEWAY-a95c4e6c041b7027c90b4803e87f5d4e",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "bc35a7e1-888c-4991-9fc2-8f2a48625c15"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-GATEWAY-BASE"
        }
      }, {
        "name" : "hive-GATEWAY-bd0a3bcd3eb72d1b8c04045035804008",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "9027ea63-0cb7-4a8d-bc04-117951411fc1"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-GATEWAY-BASE"
        }
      }, {
        "name" : "hive-GATEWAY-ffd0becf99cca5ee115a65b68ff38183",
        "type" : "GATEWAY",
        "hostRef" : {
          "hostId" : "77ed0bb6-7034-4904-9804-aa43145afb11"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-GATEWAY-BASE"
        }
      }, {
        "name" : "hive-HIVEMETASTORE-76becde789a47172e5c46b70269dfd61",
        "type" : "HIVEMETASTORE",
        "hostRef" : {
          "hostId" : "735266e9-9647-499a-a81f-4ae2b5177969"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "11mga6j173z7d69rfpw6mn04g",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-HIVEMETASTORE-BASE"
        }
      }, {
        "name" : "hive-HIVESERVER2-76becde789a47172e5c46b70269dfd61",
        "type" : "HIVESERVER2",
        "hostRef" : {
          "hostId" : "735266e9-9647-499a-a81f-4ae2b5177969"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "9nf4o67enxig9yvi5faskz5pt",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hive-HIVESERVER2-BASE"
        }
      } ],
      "displayName" : "Hive",
      "roleConfigGroups" : [ {
        "name" : "hive-GATEWAY-BASE",
        "displayName" : "Gateway Default Group",
        "roleType" : "GATEWAY",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hive"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hive-HIVEMETASTORE-BASE",
        "displayName" : "Hive Metastore Server Default Group",
        "roleType" : "HIVEMETASTORE",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hive"
        },
        "config" : {
          "items" : [ {
            "name" : "hive_metastore_java_heapsize",
            "value" : "3290431488",
            "sensitive" : false
          }, {
            "name" : "hive_metastore_server_max_message_size",
            "value" : "329043148",
            "sensitive" : false
          } ]
        }
      }, {
        "name" : "hive-HIVESERVER2-BASE",
        "displayName" : "HiveServer2 Default Group",
        "roleType" : "HIVESERVER2",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hive"
        },
        "config" : {
          "items" : [ {
            "name" : "hiveserver2_java_heapsize",
            "value" : "3290431488",
            "sensitive" : false
          }, {
            "name" : "hiveserver2_spark_driver_memory",
            "value" : "966367641",
            "sensitive" : false
          }, {
            "name" : "hiveserver2_spark_executor_cores",
            "value" : "4",
            "sensitive" : false
          }, {
            "name" : "hiveserver2_spark_executor_memory",
            "value" : "1818230784",
            "sensitive" : false
          }, {
            "name" : "hiveserver2_spark_yarn_driver_memory_overhead",
            "value" : "102",
            "sensitive" : false
          }, {
            "name" : "hiveserver2_spark_yarn_executor_memory_overhead",
            "value" : "306",
            "sensitive" : false
          } ]
        }
      }, {
        "name" : "hive-WEBHCAT-BASE",
        "displayName" : "WebHCat Server Default Group",
        "roleType" : "WEBHCAT",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hive"
        },
        "config" : {
          "items" : [ ]
        }
      } ],
      "replicationSchedules" : [ ]
    }, {
      "name" : "zookeeper",
      "type" : "ZOOKEEPER",
      "config" : {
        "items" : [ {
          "name" : "enableSecurity",
          "value" : "true",
          "sensitive" : false
        }, {
          "name" : "service_health_suppression_zookeeper_canary_health",
          "value" : "true",
          "sensitive" : false
        }, {
          "name" : "zookeeper_canary_health_enabled",
          "value" : "false",
          "sensitive" : false
        } ]
      },
      "roles" : [ {
        "name" : "zookeeper-SERVER-76becde789a47172e5c46b70269dfd61",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "735266e9-9647-499a-a81f-4ae2b5177969"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "552abx1cf6xcfzcxnc3p2kk28",
            "sensitive" : true
          }, {
            "name" : "serverId",
            "value" : "1",
            "sensitive" : false
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "zookeeper-SERVER-BASE"
        }
      }, {
        "name" : "zookeeper-SERVER-a95c4e6c041b7027c90b4803e87f5d4e",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "bc35a7e1-888c-4991-9fc2-8f2a48625c15"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "1g01tl3p4j2klj5llu06tg3ou",
            "sensitive" : true
          }, {
            "name" : "serverId",
            "value" : "2",
            "sensitive" : false
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "zookeeper-SERVER-BASE"
        }
      }, {
        "name" : "zookeeper-SERVER-bd0a3bcd3eb72d1b8c04045035804008",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "9027ea63-0cb7-4a8d-bc04-117951411fc1"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "356rzbvdcxi4on7wnr1yxh55a",
            "sensitive" : true
          }, {
            "name" : "serverId",
            "value" : "4",
            "sensitive" : false
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "zookeeper-SERVER-BASE"
        }
      }, {
        "name" : "zookeeper-SERVER-ffd0becf99cca5ee115a65b68ff38183",
        "type" : "SERVER",
        "hostRef" : {
          "hostId" : "77ed0bb6-7034-4904-9804-aa43145afb11"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "p1nv2pf61wzwiv37dlab87h6",
            "sensitive" : true
          }, {
            "name" : "serverId",
            "value" : "3",
            "sensitive" : false
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "zookeeper-SERVER-BASE"
        }
      } ],
      "displayName" : "ZooKeeper",
      "roleConfigGroups" : [ {
        "name" : "zookeeper-SERVER-BASE",
        "displayName" : "Server Default Group",
        "roleType" : "SERVER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "zookeeper"
        },
        "config" : {
          "items" : [ ]
        }
      } ]
    }, {
      "name" : "hue",
      "type" : "HUE",
      "config" : {
        "items" : [ {
          "name" : "database_host",
          "value" : "node1.gus.com",
          "sensitive" : false
        }, {
          "name" : "database_password",
          "value" : "C@paCuatro1.",
          "sensitive" : true
        }, {
          "name" : "database_type",
          "value" : "mysql",
          "sensitive" : false
        }, {
          "name" : "hive_service",
          "value" : "hive",
          "sensitive" : false
        }, {
          "name" : "hue_webhdfs",
          "value" : "hdfs-NAMENODE-76becde789a47172e5c46b70269dfd61",
          "sensitive" : false
        }, {
          "name" : "oozie_service",
          "value" : "oozie",
          "sensitive" : false
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper",
          "sensitive" : false
        } ]
      },
      "roles" : [ {
        "name" : "hue-HUE_LOAD_BALANCER-ffd0becf99cca5ee115a65b68ff38183",
        "type" : "HUE_LOAD_BALANCER",
        "hostRef" : {
          "hostId" : "77ed0bb6-7034-4904-9804-aa43145afb11"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "4aww3p7bioa0ur2tset024s3t",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hue-HUE_LOAD_BALANCER-BASE"
        }
      }, {
        "name" : "hue-HUE_SERVER-ffd0becf99cca5ee115a65b68ff38183",
        "type" : "HUE_SERVER",
        "hostRef" : {
          "hostId" : "77ed0bb6-7034-4904-9804-aa43145afb11"
        },
        "config" : {
          "items" : [ {
            "name" : "navmetadataserver_cmdb_password",
            "value" : "dbe92cdb-db6b-45a0-96bc-352d77a5b91f",
            "sensitive" : true
          }, {
            "name" : "role_jceks_password",
            "value" : "4dk78x239lxkv40t10b8p2mwn",
            "sensitive" : true
          }, {
            "name" : "secret_key",
            "value" : "09otK5qFt3pJiy5dTLvmVZaeqvPNu9",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hue-HUE_SERVER-BASE"
        }
      }, {
        "name" : "hue-KT_RENEWER-ffd0becf99cca5ee115a65b68ff38183",
        "type" : "KT_RENEWER",
        "hostRef" : {
          "hostId" : "77ed0bb6-7034-4904-9804-aa43145afb11"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "41b5w2anidx6nxlzsijmux2o9",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hue-KT_RENEWER-BASE"
        }
      } ],
      "displayName" : "Hue",
      "roleConfigGroups" : [ {
        "name" : "hue-HUE_LOAD_BALANCER-BASE",
        "displayName" : "Balancer de carga Default Group",
        "roleType" : "HUE_LOAD_BALANCER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hue"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hue-HUE_SERVER-BASE",
        "displayName" : "Hue Server Default Group",
        "roleType" : "HUE_SERVER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hue"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hue-KT_RENEWER-BASE",
        "displayName" : "Kerberos Ticket Renewer Default Group",
        "roleType" : "KT_RENEWER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hue"
        },
        "config" : {
          "items" : [ ]
        }
      } ]
    }, {
      "name" : "oozie",
      "type" : "OOZIE",
      "config" : {
        "items" : [ {
          "name" : "hive_service",
          "value" : "hive",
          "sensitive" : false
        }, {
          "name" : "mapreduce_yarn_service",
          "value" : "yarn",
          "sensitive" : false
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper",
          "sensitive" : false
        } ]
      },
      "roles" : [ {
        "name" : "oozie-OOZIE_SERVER-a95c4e6c041b7027c90b4803e87f5d4e",
        "type" : "OOZIE_SERVER",
        "hostRef" : {
          "hostId" : "bc35a7e1-888c-4991-9fc2-8f2a48625c15"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "e5htb15adl0e72e7q8hlevhtw",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "oozie-OOZIE_SERVER-BASE"
        }
      } ],
      "displayName" : "Oozie",
      "roleConfigGroups" : [ {
        "name" : "oozie-OOZIE_SERVER-BASE",
        "displayName" : "Oozie Server Default Group",
        "roleType" : "OOZIE_SERVER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "oozie"
        },
        "config" : {
          "items" : [ {
            "name" : "oozie_database_host",
            "value" : "node1.gus.com",
            "sensitive" : false
          }, {
            "name" : "oozie_database_password",
            "value" : "C@paCuatro1.",
            "sensitive" : true
          }, {
            "name" : "oozie_database_type",
            "value" : "mysql",
            "sensitive" : false
          }, {
            "name" : "oozie_database_user",
            "value" : "oozie",
            "sensitive" : false
          } ]
        }
      } ]
    }, {
      "name" : "yarn",
      "type" : "YARN",
      "config" : {
        "items" : [ {
          "name" : "hdfs_service",
          "value" : "hdfs",
          "sensitive" : false
        }, {
          "name" : "rm_dirty",
          "value" : "true",
          "sensitive" : false
        }, {
          "name" : "zk_authorization_secret_key",
          "value" : "EO1IOM6yr4PseEr225zGpEgb3Umfpi",
          "sensitive" : true
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper",
          "sensitive" : false
        } ]
      },
      "roles" : [ {
        "name" : "yarn-JOBHISTORY-a95c4e6c041b7027c90b4803e87f5d4e",
        "type" : "JOBHISTORY",
        "hostRef" : {
          "hostId" : "bc35a7e1-888c-4991-9fc2-8f2a48625c15"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "2bpb0isrn65oz6uaosh9e24qp",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-JOBHISTORY-BASE"
        }
      }, {
        "name" : "yarn-NODEMANAGER-76becde789a47172e5c46b70269dfd61",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "735266e9-9647-499a-a81f-4ae2b5177969"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "4pfawdq45knfauaxzhsjjfwx",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-NODEMANAGER-1"
        }
      }, {
        "name" : "yarn-NODEMANAGER-a95c4e6c041b7027c90b4803e87f5d4e",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "bc35a7e1-888c-4991-9fc2-8f2a48625c15"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "dz10mdfhg27qkyn400t8gvqn5",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-NODEMANAGER-BASE"
        }
      }, {
        "name" : "yarn-NODEMANAGER-ffd0becf99cca5ee115a65b68ff38183",
        "type" : "NODEMANAGER",
        "hostRef" : {
          "hostId" : "77ed0bb6-7034-4904-9804-aa43145afb11"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "dko72y8zyr0yacbmpphnk85iv",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-NODEMANAGER-2"
        }
      }, {
        "name" : "yarn-RESOURCEMANAGER-a95c4e6c041b7027c90b4803e87f5d4e",
        "type" : "RESOURCEMANAGER",
        "hostRef" : {
          "hostId" : "bc35a7e1-888c-4991-9fc2-8f2a48625c15"
        },
        "config" : {
          "items" : [ {
            "name" : "rm_id",
            "value" : "52",
            "sensitive" : false
          }, {
            "name" : "role_jceks_password",
            "value" : "4ra6xix2azi1oac2azwy92hv5",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "yarn-RESOURCEMANAGER-BASE"
        }
      } ],
      "displayName" : "YARN (MR2 Included)",
      "roleConfigGroups" : [ {
        "name" : "yarn-GATEWAY-BASE",
        "displayName" : "Gateway Default Group",
        "roleType" : "GATEWAY",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "yarn"
        },
        "config" : {
          "items" : [ {
            "name" : "mapred_reduce_tasks",
            "value" : "12",
            "sensitive" : false
          }, {
            "name" : "mapred_submit_replication",
            "value" : "3",
            "sensitive" : false
          } ]
        }
      }, {
        "name" : "yarn-JOBHISTORY-BASE",
        "displayName" : "JobHistory Server Default Group",
        "roleType" : "JOBHISTORY",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "yarn"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-1",
        "displayName" : "NodeManager Group 1",
        "roleType" : "NODEMANAGER",
        "base" : false,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "yarn"
        },
        "config" : {
          "items" : [ {
            "name" : "yarn_nodemanager_heartbeat_interval_ms",
            "value" : "100",
            "sensitive" : false
          }, {
            "name" : "yarn_nodemanager_local_dirs",
            "value" : "/mnt/resource/yarn/nm,/opt/yarn/nm",
            "sensitive" : false
          }, {
            "name" : "yarn_nodemanager_log_dirs",
            "value" : "/mnt/resource/yarn/container-logs,/opt/yarn/container-logs",
            "sensitive" : false
          }, {
            "name" : "yarn_nodemanager_resource_memory_mb",
            "value" : "4080",
            "sensitive" : false
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-2",
        "displayName" : "NodeManager Group 2",
        "roleType" : "NODEMANAGER",
        "base" : false,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "yarn"
        },
        "config" : {
          "items" : [ {
            "name" : "yarn_nodemanager_heartbeat_interval_ms",
            "value" : "100",
            "sensitive" : false
          }, {
            "name" : "yarn_nodemanager_local_dirs",
            "value" : "/mnt/resource/yarn/nm,/opt/yarn/nm",
            "sensitive" : false
          }, {
            "name" : "yarn_nodemanager_log_dirs",
            "value" : "/mnt/resource/yarn/container-logs,/opt/yarn/container-logs",
            "sensitive" : false
          }, {
            "name" : "yarn_nodemanager_resource_memory_mb",
            "value" : "11801",
            "sensitive" : false
          } ]
        }
      }, {
        "name" : "yarn-NODEMANAGER-BASE",
        "displayName" : "NodeManager Default Group",
        "roleType" : "NODEMANAGER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "yarn"
        },
        "config" : {
          "items" : [ {
            "name" : "yarn_nodemanager_heartbeat_interval_ms",
            "value" : "100",
            "sensitive" : false
          }, {
            "name" : "yarn_nodemanager_local_dirs",
            "value" : "/mnt/resource/yarn/nm,/opt/yarn/nm",
            "sensitive" : false
          }, {
            "name" : "yarn_nodemanager_log_dirs",
            "value" : "/mnt/resource/yarn/container-logs,/opt/yarn/container-logs",
            "sensitive" : false
          }, {
            "name" : "yarn_nodemanager_resource_memory_mb",
            "value" : "13644",
            "sensitive" : false
          } ]
        }
      }, {
        "name" : "yarn-RESOURCEMANAGER-BASE",
        "displayName" : "ResourceManager Default Group",
        "roleType" : "RESOURCEMANAGER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "yarn"
        },
        "config" : {
          "items" : [ {
            "name" : "yarn_scheduler_maximum_allocation_mb",
            "value" : "13644",
            "sensitive" : false
          }, {
            "name" : "yarn_scheduler_maximum_allocation_vcores",
            "value" : "8",
            "sensitive" : false
          } ]
        }
      } ]
    }, {
      "name" : "hdfs",
      "type" : "HDFS",
      "config" : {
        "items" : [ {
          "name" : "dfs_encrypt_data_transfer_algorithm",
          "value" : "AES/CTR/NoPadding",
          "sensitive" : false
        }, {
          "name" : "dfs_ha_fencing_cloudera_manager_secret_key",
          "value" : "4cB733YpEMaIeSCDX1piRoe2JGkaOs",
          "sensitive" : true
        }, {
          "name" : "fc_authorization_secret_key",
          "value" : "nZG0y5DrPkNK0ZijX5hbyb1YxlP4Kz",
          "sensitive" : true
        }, {
          "name" : "hadoop_security_authentication",
          "value" : "kerberos",
          "sensitive" : false
        }, {
          "name" : "hadoop_security_authorization",
          "value" : "true",
          "sensitive" : false
        }, {
          "name" : "http_auth_signature_secret",
          "value" : "qCIpEUw6Ejv6llt6DPdwQnsVwFkl5J",
          "sensitive" : true
        }, {
          "name" : "rm_dirty",
          "value" : "true",
          "sensitive" : false
        }, {
          "name" : "zookeeper_service",
          "value" : "zookeeper",
          "sensitive" : false
        } ]
      },
      "roles" : [ {
        "name" : "hdfs-BALANCER-76becde789a47172e5c46b70269dfd61",
        "type" : "BALANCER",
        "hostRef" : {
          "hostId" : "735266e9-9647-499a-a81f-4ae2b5177969"
        },
        "config" : {
          "items" : [ ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-BALANCER-BASE"
        }
      }, {
        "name" : "hdfs-DATANODE-76becde789a47172e5c46b70269dfd61",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "735266e9-9647-499a-a81f-4ae2b5177969"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "biaro9f1f6r9juxmhv1hzdzur",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-DATANODE-1"
        }
      }, {
        "name" : "hdfs-DATANODE-a95c4e6c041b7027c90b4803e87f5d4e",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "bc35a7e1-888c-4991-9fc2-8f2a48625c15"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "6jhz8dgv380vdtp6raamatjbw",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-DATANODE-BASE"
        }
      }, {
        "name" : "hdfs-DATANODE-ffd0becf99cca5ee115a65b68ff38183",
        "type" : "DATANODE",
        "hostRef" : {
          "hostId" : "77ed0bb6-7034-4904-9804-aa43145afb11"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "doliul3p564cnr2p2zf0bapql",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-DATANODE-BASE"
        }
      }, {
        "name" : "hdfs-FAILOVERCONTROLLER-76becde789a47172e5c46b70269dfd61",
        "type" : "FAILOVERCONTROLLER",
        "hostRef" : {
          "hostId" : "735266e9-9647-499a-a81f-4ae2b5177969"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "7yaucyi9efssy883bcxnppfgq",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-FAILOVERCONTROLLER-BASE"
        }
      }, {
        "name" : "hdfs-FAILOVERCONTROLLER-a95c4e6c041b7027c90b4803e87f5d4e",
        "type" : "FAILOVERCONTROLLER",
        "hostRef" : {
          "hostId" : "bc35a7e1-888c-4991-9fc2-8f2a48625c15"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "4ty6thw1iz2gffa7sck5b9dds",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-FAILOVERCONTROLLER-BASE"
        }
      }, {
        "name" : "hdfs-HTTPFS-ffd0becf99cca5ee115a65b68ff38183",
        "type" : "HTTPFS",
        "hostRef" : {
          "hostId" : "77ed0bb6-7034-4904-9804-aa43145afb11"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "3wkl0hji5zf958v006oqq3q0q",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-HTTPFS-BASE"
        }
      }, {
        "name" : "hdfs-JOURNALNODE-76becde789a47172e5c46b70269dfd61",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "735266e9-9647-499a-a81f-4ae2b5177969"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "704zhh25xakj61qjbxfjfhjwa",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-JOURNALNODE-BASE"
        }
      }, {
        "name" : "hdfs-JOURNALNODE-bd0a3bcd3eb72d1b8c04045035804008",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "9027ea63-0cb7-4a8d-bc04-117951411fc1"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "ze47vxvs2g5e3oyfuujzyjkk",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-JOURNALNODE-BASE"
        }
      }, {
        "name" : "hdfs-JOURNALNODE-ffd0becf99cca5ee115a65b68ff38183",
        "type" : "JOURNALNODE",
        "hostRef" : {
          "hostId" : "77ed0bb6-7034-4904-9804-aa43145afb11"
        },
        "config" : {
          "items" : [ {
            "name" : "role_jceks_password",
            "value" : "3o5t3wf25x98pfqw7y6rk45hd",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-JOURNALNODE-BASE"
        }
      }, {
        "name" : "hdfs-NAMENODE-76becde789a47172e5c46b70269dfd61",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "735266e9-9647-499a-a81f-4ae2b5177969"
        },
        "config" : {
          "items" : [ {
            "name" : "autofailover_enabled",
            "value" : "true",
            "sensitive" : false
          }, {
            "name" : "dfs_federation_namenode_nameservice",
            "value" : "nameservice1",
            "sensitive" : false
          }, {
            "name" : "dfs_namenode_quorum_journal_name",
            "value" : "nameservice1",
            "sensitive" : false
          }, {
            "name" : "namenode_id",
            "value" : "54",
            "sensitive" : false
          }, {
            "name" : "role_jceks_password",
            "value" : "daq8q1rb4go4jqef19h83j2jd",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-NAMENODE-BASE"
        }
      }, {
        "name" : "hdfs-NAMENODE-a95c4e6c041b7027c90b4803e87f5d4e",
        "type" : "NAMENODE",
        "hostRef" : {
          "hostId" : "bc35a7e1-888c-4991-9fc2-8f2a48625c15"
        },
        "config" : {
          "items" : [ {
            "name" : "autofailover_enabled",
            "value" : "true",
            "sensitive" : false
          }, {
            "name" : "dfs_federation_namenode_nameservice",
            "value" : "nameservice1",
            "sensitive" : false
          }, {
            "name" : "dfs_namenode_quorum_journal_name",
            "value" : "nameservice1",
            "sensitive" : false
          }, {
            "name" : "namenode_id",
            "value" : "60",
            "sensitive" : false
          }, {
            "name" : "role_jceks_password",
            "value" : "djm2qb6hjzrs0zjp9fy1tbluy",
            "sensitive" : true
          } ]
        },
        "roleConfigGroupRef" : {
          "roleConfigGroupName" : "hdfs-NAMENODE-BASE"
        }
      } ],
      "displayName" : "HDFS",
      "roleConfigGroups" : [ {
        "name" : "hdfs-BALANCER-BASE",
        "displayName" : "Balancer Default Group",
        "roleType" : "BALANCER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hdfs-DATANODE-1",
        "displayName" : "DataNode Group 1",
        "roleType" : "DATANODE",
        "base" : false,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ {
            "name" : "dfs_data_dir_list",
            "value" : "/mnt/resource/dfs/dn,/opt/dfs/dn",
            "sensitive" : false
          }, {
            "name" : "dfs_datanode_data_dir_perm",
            "value" : "700",
            "sensitive" : false
          }, {
            "name" : "dfs_datanode_failed_volumes_tolerated",
            "value" : "1",
            "sensitive" : false
          }, {
            "name" : "dfs_datanode_http_port",
            "value" : "1006",
            "sensitive" : false
          }, {
            "name" : "dfs_datanode_max_locked_memory",
            "value" : "4278190080",
            "sensitive" : false
          }, {
            "name" : "dfs_datanode_port",
            "value" : "1004",
            "sensitive" : false
          } ]
        }
      }, {
        "name" : "hdfs-DATANODE-BASE",
        "displayName" : "DataNode Default Group",
        "roleType" : "DATANODE",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ {
            "name" : "dfs_data_dir_list",
            "value" : "/mnt/resource/dfs/dn,/opt/dfs/dn",
            "sensitive" : false
          }, {
            "name" : "dfs_datanode_data_dir_perm",
            "value" : "700",
            "sensitive" : false
          }, {
            "name" : "dfs_datanode_failed_volumes_tolerated",
            "value" : "1",
            "sensitive" : false
          }, {
            "name" : "dfs_datanode_http_port",
            "value" : "1006",
            "sensitive" : false
          }, {
            "name" : "dfs_datanode_port",
            "value" : "1004",
            "sensitive" : false
          } ]
        }
      }, {
        "name" : "hdfs-FAILOVERCONTROLLER-BASE",
        "displayName" : "Failover Controller Default Group",
        "roleType" : "FAILOVERCONTROLLER",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hdfs-GATEWAY-BASE",
        "displayName" : "Gateway Default Group",
        "roleType" : "GATEWAY",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ {
            "name" : "dfs_client_use_trash",
            "value" : "true",
            "sensitive" : false
          } ]
        }
      }, {
        "name" : "hdfs-HTTPFS-BASE",
        "displayName" : "HttpFS Default Group",
        "roleType" : "HTTPFS",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hdfs-JOURNALNODE-BASE",
        "displayName" : "JournalNode Default Group",
        "roleType" : "JOURNALNODE",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ {
            "name" : "dfs_journalnode_edits_dir",
            "value" : "/opt/dfs/jn",
            "sensitive" : false
          } ]
        }
      }, {
        "name" : "hdfs-NAMENODE-BASE",
        "displayName" : "NameNode Default Group",
        "roleType" : "NAMENODE",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ {
            "name" : "dfs_name_dir_list",
            "value" : "/mnt/resource/dfs/nn,/opt/dfs/nn",
            "sensitive" : false
          }, {
            "name" : "dfs_namenode_servicerpc_address",
            "value" : "8022",
            "sensitive" : false
          }, {
            "name" : "namenode_java_heapsize",
            "value" : "3290431488",
            "sensitive" : false
          } ]
        }
      }, {
        "name" : "hdfs-NFSGATEWAY-BASE",
        "displayName" : "NFS Gateway Default Group",
        "roleType" : "NFSGATEWAY",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ ]
        }
      }, {
        "name" : "hdfs-SECONDARYNAMENODE-BASE",
        "displayName" : "SecondaryNameNode Default Group",
        "roleType" : "SECONDARYNAMENODE",
        "base" : true,
        "serviceRef" : {
          "clusterName" : "cluster",
          "serviceName" : "hdfs"
        },
        "config" : {
          "items" : [ {
            "name" : "fs_checkpoint_dir_list",
            "value" : "/mnt/resource/dfs/snn",
            "sensitive" : false
          }, {
            "name" : "secondary_namenode_java_heapsize",
            "value" : "3290431488",
            "sensitive" : false
          } ]
        }
      } ],
      "replicationSchedules" : [ ],
      "snapshotPolicies" : [ ]
    } ],
    "parcels" : [ {
      "product" : "CDH",
      "version" : "5.12.1-1.cdh5.12.1.p0.3",
      "stage" : "DISTRIBUTED",
      "clusterRef" : {
        "clusterName" : "cluster"
      }
    }, {
      "product" : "CDH",
      "version" : "5.12.1-1.cdh5.12.1.p0.3",
      "stage" : "ACTIVATED",
      "clusterRef" : {
        "clusterName" : "cluster"
      }
    } ],
    "uuid" : "a0264658-58ee-4645-b862-2bedcd9f21fc"
  } ],
  "hosts" : [ {
    "hostId" : "9027ea63-0cb7-4a8d-bc04-117951411fc1",
    "ipAddress" : "10.0.0.110",
    "hostname" : "node1.gus.com",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "735266e9-9647-499a-a81f-4ae2b5177969",
    "ipAddress" : "10.0.0.102",
    "hostname" : "node2.gus.com",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "77ed0bb6-7034-4904-9804-aa43145afb11",
    "ipAddress" : "10.0.0.103",
    "hostname" : "node3.gus.com",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  }, {
    "hostId" : "bc35a7e1-888c-4991-9fc2-8f2a48625c15",
    "ipAddress" : "10.0.0.104",
    "hostname" : "node4.gus.com",
    "rackId" : "/default",
    "config" : {
      "items" : [ ]
    }
  } ],
  "users" : [ {
    "name" : "GustavoAco",
    "roles" : [ "ROLE_ADMIN" ],
    "pwHash" : "55565aa5ed2ac0d1986186f01cc654b13a072a5aab78d29b1ef2906c90f95328",
    "pwSalt" : -8548871980790895218,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__hue-HUE_SERVER-ffd0becf99cca5ee115a65b68ff38183",
    "roles" : [ "ROLE_NAVIGATOR_ADMIN" ],
    "pwHash" : "9faf2ea0350a95a861f22f051c6790634eed225e23a7deb3e2d2ec18fe8ffd62",
    "pwSalt" : 37376098395436460,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-EVENTSERVER-bd0a3bcd3eb72d1b8c04045035804008",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "54ba3968be8103889431cd3e515cb49c6e8aca17d5dabfc2373d9ee5911c6672",
    "pwSalt" : 3857203180564191345,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-HOSTMONITOR-bd0a3bcd3eb72d1b8c04045035804008",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "2b5a3e844eb12cf20750a48a86b9f9936956f8cce8bb4f0bb8dfac30a708426e",
    "pwSalt" : -4452257315302895482,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-REPORTSMANAGER-bd0a3bcd3eb72d1b8c04045035804008",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "ecd4dc3d67ec7b462f37201aa8b907a2f0eeeb6a22b05ce0385c0d27cb3fa7b7",
    "pwSalt" : -2261164758882278723,
    "pwLogin" : true
  }, {
    "name" : "__cloudera_internal_user__mgmt-SERVICEMONITOR-bd0a3bcd3eb72d1b8c04045035804008",
    "roles" : [ "ROLE_USER" ],
    "pwHash" : "02f90cc32354500710a48166709285a41e5a52bd1e2c6d53ee96347ce516c493",
    "pwSalt" : 7601640362067448460,
    "pwLogin" : true
  }, {
    "name" : "admin",
    "roles" : [ "ROLE_ADMIN" ],
    "pwHash" : "1894ea4c7f10fbb869d4247a643739e0c5ef3cb4df6b4440657e4ac2f4584173",
    "pwSalt" : -6058590561447782457,
    "pwLogin" : true
  } ],
  "versionInfo" : {
    "version" : "5.12.1",
    "buildUser" : "jenkins",
    "buildTimestamp" : "20170818-0807",
    "gitHash" : "9bdee611802535491d400e03c98ef694a2c77d0a",
    "snapshot" : false
  },
  "managementService" : {
    "name" : "mgmt",
    "type" : "MGMT",
    "config" : {
      "items" : [ ]
    },
    "roles" : [ {
      "name" : "mgmt-ALERTPUBLISHER-bd0a3bcd3eb72d1b8c04045035804008",
      "type" : "ALERTPUBLISHER",
      "hostRef" : {
        "hostId" : "9027ea63-0cb7-4a8d-bc04-117951411fc1"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "e8b7rufa079qn46s145hzvv5d",
          "sensitive" : true
        } ]
      },
      "roleConfigGroupRef" : {
        "roleConfigGroupName" : "mgmt-ALERTPUBLISHER-BASE"
      }
    }, {
      "name" : "mgmt-EVENTSERVER-bd0a3bcd3eb72d1b8c04045035804008",
      "type" : "EVENTSERVER",
      "hostRef" : {
        "hostId" : "9027ea63-0cb7-4a8d-bc04-117951411fc1"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "2de3plqyhdszyg4ox6fua30zb",
          "sensitive" : true
        } ]
      },
      "roleConfigGroupRef" : {
        "roleConfigGroupName" : "mgmt-EVENTSERVER-BASE"
      }
    }, {
      "name" : "mgmt-HOSTMONITOR-bd0a3bcd3eb72d1b8c04045035804008",
      "type" : "HOSTMONITOR",
      "hostRef" : {
        "hostId" : "9027ea63-0cb7-4a8d-bc04-117951411fc1"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "bp8u5phk28i1rw8h8rhw36a2e",
          "sensitive" : true
        } ]
      },
      "roleConfigGroupRef" : {
        "roleConfigGroupName" : "mgmt-HOSTMONITOR-BASE"
      }
    }, {
      "name" : "mgmt-REPORTSMANAGER-bd0a3bcd3eb72d1b8c04045035804008",
      "type" : "REPORTSMANAGER",
      "hostRef" : {
        "hostId" : "9027ea63-0cb7-4a8d-bc04-117951411fc1"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "64an516766faxmjtxzuifj84p",
          "sensitive" : true
        } ]
      },
      "roleConfigGroupRef" : {
        "roleConfigGroupName" : "mgmt-REPORTSMANAGER-BASE"
      }
    }, {
      "name" : "mgmt-SERVICEMONITOR-bd0a3bcd3eb72d1b8c04045035804008",
      "type" : "SERVICEMONITOR",
      "hostRef" : {
        "hostId" : "9027ea63-0cb7-4a8d-bc04-117951411fc1"
      },
      "config" : {
        "items" : [ {
          "name" : "role_jceks_password",
          "value" : "17oj884o3k2w0todbbi6gor8t",
          "sensitive" : true
        } ]
      },
      "roleConfigGroupRef" : {
        "roleConfigGroupName" : "mgmt-SERVICEMONITOR-BASE"
      }
    } ],
    "displayName" : "Cloudera Management Service",
    "roleConfigGroups" : [ {
      "name" : "mgmt-ACTIVITYMONITOR-BASE",
      "displayName" : "Activity Monitor Default Group",
      "roleType" : "ACTIVITYMONITOR",
      "base" : true,
      "serviceRef" : {
        "serviceName" : "mgmt"
      },
      "config" : {
        "items" : [ ]
      }
    }, {
      "name" : "mgmt-ALERTPUBLISHER-BASE",
      "displayName" : "Alert Publisher Default Group",
      "roleType" : "ALERTPUBLISHER",
      "base" : true,
      "serviceRef" : {
        "serviceName" : "mgmt"
      },
      "config" : {
        "items" : [ ]
      }
    }, {
      "name" : "mgmt-EVENTSERVER-BASE",
      "displayName" : "Event Server Default Group",
      "roleType" : "EVENTSERVER",
      "base" : true,
      "serviceRef" : {
        "serviceName" : "mgmt"
      },
      "config" : {
        "items" : [ ]
      }
    }, {
      "name" : "mgmt-HOSTMONITOR-BASE",
      "displayName" : "Host Monitor Default Group",
      "roleType" : "HOSTMONITOR",
      "base" : true,
      "serviceRef" : {
        "serviceName" : "mgmt"
      },
      "config" : {
        "items" : [ {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "1610612736",
          "sensitive" : false
        } ]
      }
    }, {
      "name" : "mgmt-NAVIGATOR-BASE",
      "displayName" : "Navigator Audit Server Default Group",
      "roleType" : "NAVIGATOR",
      "base" : true,
      "serviceRef" : {
        "serviceName" : "mgmt"
      },
      "config" : {
        "items" : [ ]
      }
    }, {
      "name" : "mgmt-NAVIGATORMETASERVER-BASE",
      "displayName" : "Navigator Metadata Server Default Group",
      "roleType" : "NAVIGATORMETASERVER",
      "base" : true,
      "serviceRef" : {
        "serviceName" : "mgmt"
      },
      "config" : {
        "items" : [ ]
      }
    }, {
      "name" : "mgmt-REPORTSMANAGER-BASE",
      "displayName" : "Reports Manager Default Group",
      "roleType" : "REPORTSMANAGER",
      "base" : true,
      "serviceRef" : {
        "serviceName" : "mgmt"
      },
      "config" : {
        "items" : [ {
          "name" : "headlamp_database_host",
          "value" : "node1.gus.com",
          "sensitive" : false
        }, {
          "name" : "headlamp_database_name",
          "value" : "rman",
          "sensitive" : false
        }, {
          "name" : "headlamp_database_password",
          "value" : "C@paCuatro1.",
          "sensitive" : true
        }, {
          "name" : "headlamp_database_user",
          "value" : "rman",
          "sensitive" : false
        } ]
      }
    }, {
      "name" : "mgmt-SERVICEMONITOR-BASE",
      "displayName" : "Service Monitor Default Group",
      "roleType" : "SERVICEMONITOR",
      "base" : true,
      "serviceRef" : {
        "serviceName" : "mgmt"
      },
      "config" : {
        "items" : [ {
          "name" : "firehose_non_java_memory_bytes",
          "value" : "1610612736",
          "sensitive" : false
        } ]
      }
    }, {
      "name" : "mgmt-TELEMETRYPUBLISHER-BASE",
      "displayName" : "Telemetry Publisher Default Group",
      "roleType" : "TELEMETRYPUBLISHER",
      "base" : true,
      "serviceRef" : {
        "serviceName" : "mgmt"
      },
      "config" : {
        "items" : [ ]
      }
    } ]
  },
  "managerSettings" : {
    "items" : [ {
      "name" : "AD_USE_SIMPLE_AUTH",
      "value" : "false",
      "sensitive" : false
    }, {
      "name" : "CLUSTER_STATS_START",
      "value" : "10/22/2012 11:30",
      "sensitive" : false
    }, {
      "name" : "KDC_ADMIN_HOST",
      "value" : "node1.gus.com",
      "sensitive" : false
    }, {
      "name" : "KDC_ADMIN_PASSWORD",
      "value" : "BQIAAAA6AAEAB0dVUy5DT00ADGNsb3VkZXJhLXNjbQAAAAFaIDvrAQAXABAKyB2Zj+AJO7VTAzmLJ0ZQAAAAAQ==",
      "sensitive" : true
    }, {
      "name" : "KDC_ADMIN_USER",
      "value" : "cloudera-scm@GUS.COM",
      "sensitive" : false
    }, {
      "name" : "KDC_HOST",
      "value" : "node1.gus.com",
      "sensitive" : false
    }, {
      "name" : "KRB_ENC_TYPES",
      "value" : "arcfour-hmac",
      "sensitive" : false
    }, {
      "name" : "KRB_MANAGE_KRB5_CONF",
      "value" : "true",
      "sensitive" : false
    }, {
      "name" : "MAX_RENEW_LIFE",
      "value" : "604800",
      "sensitive" : false
    }, {
      "name" : "PUBLIC_CLOUD_STATUS",
      "value" : "NOT_ON_PUBLIC_CLOUD",
      "sensitive" : false
    }, {
      "name" : "REMOTE_PARCEL_REPO_URLS",
      "value" : "https://archive.cloudera.com/cdh5/parcels/{latest_supported}/,https://archive.cloudera.com/cdh4/parcels/latest/,https://archive.cloudera.com/impala/parcels/latest/,https://archive.cloudera.com/search/parcels/latest/,https://archive.cloudera.com/accumulo/parcels/1.4/,https://archive.cloudera.com/accumulo-c5/parcels/latest/,https://archive.cloudera.com/kafka/parcels/latest/,http://archive.cloudera.com/kudu/parcels/latest/,https://archive.cloudera.com/spark/parcels/latest/,https://archive.cloudera.com/sqoop-connectors/parcels/latest/",
      "sensitive" : false
    }, {
      "name" : "SECURITY_REALM",
      "value" : "GUS.COM",
      "sensitive" : false
    } ]
  },
  "allHostsConfig" : {
    "items" : [ ]
  },
  "peers" : [ ],
  "hostTemplates" : {
    "items" : [ ]
  }
}

```
