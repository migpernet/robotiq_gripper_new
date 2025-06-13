No arquivo urdf para plugin mimmic adicionei esse trecho de script:

<!-- adicionei o plugin para o robotiq_right_finger_joint -->
  <plugin filename="libroboticsgroup_upatras_gazebo_mimic_joint_plugin.so" name="${prefix}mimic_robotiq_85_3">
      <joint>${prefix}robotiq_85_left_knuckle_joint</joint>
      <mimicJoint>${prefix}robotiq_85_right_finger_joint</mimicJoint>
      <multiplier>0.0</multiplier>
      <!--offset>0.0</offset-->
  </plugin>

  <!-- adicionei o plugin para o robotiq_left_finger_joint -->
  <plugin filename="libroboticsgroup_upatras_gazebo_mimic_joint_plugin.so" name="${prefix}mimic_robotiq_85_3">
      <joint>${prefix}robotiq_85_left_knuckle_joint</joint>
      <mimicJoint>${prefix}robotiq_85_left_finger_joint</mimicJoint>
      <multiplier>0.0</multiplier>
      <!--offset>0.0</offset-->
  </plugin>
