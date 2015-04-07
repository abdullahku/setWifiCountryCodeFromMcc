.line 189
    .local v3, "locale":Ljava/util/Locale;
    if-eqz v4, :cond_0

    .line 190
    invoke-static {p0, v4}, Lcom/android/internal/telephony/MccTable;->setTimezoneFromMccIfNeeded(Landroid/content/Context;I)V

    .line 191
    invoke-static {p0, v4}, Lcom/android/internal/telephony/MccTable;->getLocaleFromMcc(Landroid/content/Context;I)Ljava/util/Locale;

    move-result-object v3

    .line 193
    :cond_0
    if-eqz p2, :cond_2

    .line 225
    .end local v1    # "defaultMccMnc":Ljava/lang/String;
    .end local v3    # "locale":Ljava/util/Locale;
    .end local v4    # "mcc":I
    .end local v5    # "mnc":I
    :cond_1
    :goto_0
    return-void
