# Ganesh-Kumar
============================Script for Delivery==============================================
delivery.operation_id=instance.operation_id;
delivery.workflow_id=instance.id;
=============================================================================================

=====================================Campaign Naming=========================================
NIMF_Investor/Distributor_CampaignType_CampaignName_MonthYear_Campaign
=============================================================================================

=====================================Workflow Naming=========================================
NIMF_Investor/Distributor_CampaignType_CampaignChannel_CampaignName_MonthYear_WaveNumber
=============================================================================================

=====================================Delivery Naming=========================================
NIMF_Investor/Distributor_CampaignType_CampaignChannel_CampaignName_MonthYear_Segment_waveNumber
=============================================================================================

=====================================Import Naming=========================================
NIMF_Investor/Distributor_FileName_FileDate_ImportDate
=============================================================================================

=====================================Mirror Page=============================================
<center><%@ include view='MirrorPage' %></center>
=============================================================================================

=====================================Unsubscribe Link========================================
<tr>
<td height="25" style="font-family:Arial, Helvetica, sans-serif, Helvetica, sans-serif, Helvetica, sans-serif; font-size:12px; text-align:left; line-height:15px; color:#000000">
<center><%@ include view='PVIEW6' %></center>
</td>
</tr>
=============================================================================================

=====================================Waterfall Script========================================
vars.Table1Count= vars.recCount;  //------For Activity Count
vars.Table1Label = activity.label;  //------For Activity Label
vars.WorkflowLabel=instance.label //---- for workflowlabel
vars.Table2Count= vars.recCount;  //------For Activity Count
vars.Table2Label = activity.label;  //------For Activity Label

=============================================================================================
=====================================Waterfall Alert Code====================================
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.0 Transitional//EN">
<HTML><HEAD>
<STYLE>
table, th, td {
  border: 1px solid black;
  border-radius: 10px;
}
</STYLE>

<META name=GENERATOR content="MSHTML 11.00.9600.20139"></HEAD>
<BODY><BR><BR>
<CENTER>
<H1>Nippon Waterfall</H1></CENTER>
<TABLE style="WIDTH: 100%" border=2>
  <TBODY>
      <TR bgColor="#ffff00">
    <TH colSpan=2><%= instance.label %> Waterfall</TH>
    </TR>
  <TR bgColor=orange>
    <TH>Activity</TH>
    <TH>Count</TH></TR>
  <TR>
    <TD><%= vars.Table1Label %> </TD>
    <TD><%= vars.Table1Count %></TD>
  </TR>
  <TR>
    <TD><%= vars.Table2Label %></TD>
    <TD><%= vars.Table2Count %></TD>
  </TR>
  <TR>
    <TD><%= vars.Table3Label %></TD>
    <TD><%= vars.Table3Count %></TD>
  </TR>
  <TR>
    <TD><%= vars.Table4Label %></TD>
    <TD><%= vars.Table4Count %></TD>
  </TR>
    <TR>
    <TD><%= vars.Table5Label %></TD>
    <TD><%= vars.Table5Count %></TD>
  </TR>
    <TR>
    <TD><%= vars.Table6Label %></TD>
    <TD><%= vars.Table6Count %></TD>
  </TR>
    <TR>
    <TD><%= vars.Table7Label %></TD>
    <TD><%= vars.Table7Count %></TD>
  </TR>
    <TR>
    <TD><%= vars.Table8Label %></TD>
    <TD><%= vars.Table8Count %></TD>
  </TR>
    <TR>
    <TD><%= vars.Table9Label %></TD>
    <TD><%= vars.Table9Count %></TD>
  </TR>
    <TR>
    <TD><%= vars.Table10Label %></TD>
    <TD><%= vars.Table10Count %></TD>
  </TR>
  <TR bgColor="#2bff00">
    <TH>Final Count</TH>
    <TH><%= vars.Table10Count %></TH>
    </TR>
    </TBODY>
    </TABLE>
    </BODY>
    </HTML>
=============================================================================================
