STEPS_DIR := tutorial-steps
DEV_OUTPUTS_DIR := $(STEPS_DIR)/dev/outputs
TEMP_DIR := $(shell mktemp -d)
SEQUENCE := "dev, test, prod, ccloud"

tutorial:
	harness-runner ../../../../../_data/harnesses/kafka-connect-datagen-ccloud/kafka.yml $(TEMP_DIR) $(SEQUENCE)
	reset
